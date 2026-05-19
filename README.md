# NodeSynth

Tool Prototype: https://support-tickets-29m1bnjrfkk.streamlit.app/

NodeSynth is a research prototype that implements a scalable, multi-stage
method for creating socially relevant and grounded synthetic data (e.g.,
annotated queries) for AI model evaluation. The pipeline breaks down topics
related to safety policies (e.g., harassment) and sensitive domains (e.g.,
education) into taxonomies using a fine-tuned taxonomy generator; identifies
key relationships within the taxonomies (e.g., social groups, use cases); and
validates synthetic query quality for model evaluation.

NodeSynth enables users (e.g., researchers, developers) to go from a topic to a
synthetic dataset capturing relationships that represent documented harms in the
real world. This prototype and the approach outlined in the accompanying paper
can be used to conduct lightweight model evaluations specific to sensitive
topics, enabling model developers and deployers to prioritize key areas of
concern for in-depth human evaluation.

## Learn More
To learn more about NodeSynth and relevant experiments, read the paper: https://arxiv.org/abs/2605.14381.  

## Citation

If you use NodeSynth in your research, please cite the following paper:

@article{rashid2026nodesynth,
  title={NodeSynth: Socially Aligned Synthetic Data for AI Evaluation},
  author={Rashid, Qazi Mamunur and Yang, Xuan and Yang, Zhengzhe and Pan, Yanzhou and van Liemt, Erin and Neal, Darlene and Pancholi, Kshitij and Smith-Loud, Jamila},
  journal={arXiv preprint arXiv:2605.14381},
  year={2026}
}

## Disclaimer

This is not an officially supported Google product. This project is not
eligible for the [Google Open Source Software Vulnerability Rewards
Program](https://bughunters.google.com/open-source-security).

This project is intended for demonstration purposes only. It is not
intended for use in a production environment.

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## Contributing

See [`CONTRIBUTING.md`](CONTRIBUTING.md) for details.

## How to run it on your own machine

python3 -m venv venv;
source venv/bin/activate;
pip install -r requirements.txt;
streamlit run streamlit_app.py;
