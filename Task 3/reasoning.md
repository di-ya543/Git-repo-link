1. Why is this model better suitable for high-level semantic meaning?

I choose CodeT5 because it is trained specifically on source code in multiple languages, including Python. Unlike simple syntax checkers, it learns semantic meaning, i.e., the logic and intent behind code, not just surface-level structure. This makes it more suitable for high-level competence analysis since it can identify conceptual mistakes (e.g., using the wrong algorithm) rather than just syntax errors.

2. What trade-offs might occur when a model generates meaningful prompts?

Accuracy vs. Simplicity: A highly detailed explanation may overwhelm beginners, while oversimplified hints may not help advanced learners.

Interpretability vs. Generality: Models that generate rich prompts may use technical jargon that is hard for students to understand.

Performance vs. Resource Use: Larger models like CodeT5 require significant compute resources, which may limit classroom adoption.

3. How would you address those trade-offs?

For accuracy vs. simplicity, I would adapt the model’s outputs to the student’s level (beginner vs. advanced) by controlling explanation depth.

For interpretability, I would design a post-processing step that rephrases technical hints into simpler, student-friendly language.

For performance issues, I would use smaller distilled versions of the model (e.g., CodeT5-small) to ensure faster inference while retaining educational value.
