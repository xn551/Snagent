# Snagent
Snagent or Sneke-Agent is a Python-written LLM agent that operates entirely with Python. Unlike Openclaw, this project aims to deploy multiple medium-sized LLMs (e.g., 20B or 30B models, or even smaller ones) locally. Therefore, the multi-agents is named Tiny-Snekes, in contrast to large models with ~1000B parameters.

However, to enhance multi-agent capability, Snake-Agent needs to cooperate. These agents have distinct roles, such as Operator, Planner, Coder, Adviser, Executor, Secretary, Reviewer, Summarizer, Evaluator (HR), and others. Each role is assigned its own system prompts, configuration options, and retains independent context with differentiated permissions. For example, only the Secretary can create directories or files in the sandbox environment, while only the Executor is authorized to execute files built by the Secretary.

The core principle is to leverage Sneke-Agents for mutual evaluation, analogous to the generator and discriminator in a GAN (Generative Adversarial Network), but designed to mimic human-like behavior. To mitigate biases or hallucinations inherent in mid-scale AI models, different role-class(Sneke-Agnet) should select different models, especially for worker-roles (e.g., Planner, Coder) versus supervisory-roles (e.g., Reviewer, Evaluator).

## Project Progress
- 2026-3-9 Added the submodule Snako, a cartoon LLM chat interface. Available in https://github.com/xn551/Sneko
