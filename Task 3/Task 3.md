Research Plan: Evaluating Open Source Models for Student Competence Analysis

Approach to Evaluation

To evaluate open-source AI models for student competence analysis, I would begin by identifying models that are:

Freely available and actively maintained (e.g., Hugging Face models like CodeT5, GPT-J, or educational NLP frameworks).

Designed for code analysis, NLP, or educational tasks.


The evaluation process would include:

1. Reviewing the model’s documentation and intended use cases.


2. Testing the model with student-written Python code samples (containing common mistakes).


3. Observing whether the model can analyze logic, detect misconceptions, and prompt students with constructive guidance instead of direct answers.

Criteria for Suitability :-

A model is suitable for high-level competence analysis if it:

Understands code structure (syntax + logic).

Identifies misconceptions or reasoning gaps.

Generates hints that encourage problem-solving instead of spoon-feeding answers.

Maintains interpretability (clear outputs) and is lightweight enough to be practical in an educational setting.

Testing and Validation :-

I would validate applicability by:

Running the model on a dataset of buggy Python programs from beginner/intermediate students.

Measuring whether its feedback:

Identifies the mistake.

Provides useful, constructive prompts.

Avoids giving away the direct solution.


Comparing feedback quality against human tutor responses for alignment.

Reasoning and Decision-Making :-

I chose CodeT5 (Hugging Face) as an example candidate because it is an open-source transformer model specialized for code understanding and generation.

Strengths:

Trained on multiple programming languages, including Python.

Strong at analyzing syntax and semantics.

Freely available and supported by a large community.


Limitations:

May produce overly technical hints that are difficult for beginners.

Requires careful fine-tuning to adapt for educational guidance instead of pure code correction.


Trade-offs Considered :-

Accuracy vs. Interpretability: More complex models (like GPT-J) may give highly accurate analysis but produce explanations that are hard for students to follow.

Performance vs. Cost: Larger models provide better insights but require higher compute power, which may not be feasible in resource-limited classrooms.

Generality vs. Specificity: Some models may work across all programming languages but lack fine-tuned feedback for Python-specific learning patterns.
