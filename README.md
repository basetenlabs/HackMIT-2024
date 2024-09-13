# HackMIT Baseten Info

Hi Hackers!

We're super excited to be with you here this weekend at HackMIT. This repository contains everything you need to know to use Baseten for your AI-powered projects.

## What is Baseten?

Baseten is an inference-focused AI infrastructure platform that powers mission-critical production workloads for best-in-class AI-native startups like Descript, Bland, and Writer. We're a series B company with offices in SF and NY and teammates around the world.

Or, for the purposes of this hackathon, Baseten is a place for you to get free GPUs and free inference on state-of-the-art AI models.

## How do I use Baseten?

Baseten is built for production inference on AI models. With Baseten, you can build a model server for any open-source model from Hugging Face or even your own fine-tuned models and serve it behind and autoscaling API endpoint.

However, for this hackathon, we've also set up a few shared endpoints to make it easier to get started.

### Quickstart model endpoints

We're big believers in dedicated deployments at Baseten. Dedicated deployments are more robust, scalable, reliable, and secure than shared inference endpoints (e.g. the OpenAI ChatCompletions API).

However, at a hackathon, dedicated deployments can be a bit inefficient, as every team spins up their own deployment of the model only to use a small fraction of its capacity. To address this, I've created shared endpoints for three popular models within my own Baseten account.

You are still encouraged to deploy your own models as well!

#### How do I get an API key?

Within my own Baseten account, I've deployed the models and created read-only API keys that will allow you to run inference on the models. I have autoscaling set up, but please be nice and don't slam the models, these are a shared resource.

The shared inference endpoint API key is: 

**IMPORTANT**: these models will only be live for the hackathon through end of day Sunday. Each model notebook has a link to deploy the model for yourself if you want to use it after the project, all you'll need to do is swap out the model ID and API key.

#### What models did you set up endpoints for?

Models:

* Llama 3.1 (chat) in `01_llama.ipynb`.
* FLUX.1 (image generation) in `02_flux.ipynb`.
* Whisper 3 (transcription) in `03_whisper.ipynb`.

### DIY deployment

Want a different model? No problem at all. Use this:

* [Model library](https://www.baseten.co/library/)
* Supported LLMs (fine-tunes of Llama and Mistral): [TensorRT-LLM Engine Builder](https://docs.baseten.co/performance/engine-builder-overview)
* All models: Truss
  * [Truss docs](https://docs.baseten.co/deploy/overview)
  * [Truss tutorial](https://docs.baseten.co/quickstart)
  * [Truss examples](https://github.com/basetenlabs/truss-examples)
* Compound AI systems: [Chains](https://docs.baseten.co/chains/overview)


## How can I get help?

For technical issues, start with the [documentation](https://docs.baseten.co), which has a handy built-in LLM chat with full docs access.

For additional free credits, send an email to philip.kiely@baseten.co with your workspace email and a quick sentence about what you need the credits for.

For everything else, Philip and Mike from Baseten will be on-site Saturday and Sunday to help with any issues. Look for us at the sponsor table!
