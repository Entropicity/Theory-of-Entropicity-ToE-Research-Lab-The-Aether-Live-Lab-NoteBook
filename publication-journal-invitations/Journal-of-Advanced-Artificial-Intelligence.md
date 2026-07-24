# Journal of Advanced Artificial Intelligence



---------- Forwarded message ---------

From: Editor <editorial.workflow@mail.wren-research-journals.com>

Date: Wed, Apr 29, 2026, 2:12 AM

Subject: Invitation to review

To: John Onimisi Obidi <jonimisiobidi@gmail.com>


Dear Dr. John Onimisi Obidi,

I believe that you would serve as an excellent reviewer for a submission to Journal of Advanced Artificial Intelligence, Engineering and Technology. The submission's title and abstract are below, and I hope that you will consider undertaking this important task for us.

If you are able to review this submission, your review is due by 2026-05-04. You can view the submission, upload review files, and submit your review by logging into the journal site and following the steps at the link below.

## Angle Domain Gaussian Perturbations via Ancilla Hamming Weight

### Abstract

We introduce a quantum circuit that works in the angle domain to generate local,
approximately Gaussian perturbations around a given vector. 

Instead of encoding
a full distribution into quantum amplitudes, our method operates directly on
rotation angles, making it better suited for localized perturbations rather than
global distribution loading.

For each feature qubit, we add m ancilla qubits prepared in the |+⟩ state and
apply the same controlled Ry(α) rotation from each of them. Together, these
rotations create a shift that depends on the number of ancillas measured in the
state |1⟩ (the Hamming weight W). 

After applying a centering correction, the
resulting perturbation follows a discrete distribution:

x′ = x +αaW −m2, 

W ∼ Binomial(m, 12 ).

We derive closed-form expressions for the mean and variance of the perturbation
and show that selecting

α = 2aσ√m

yields a target variance σ2. While the finite-m distribution is discrete, it converges
to a Gaussian distribution under standardization via the Central Limit
Theorem, with approximation error governed by Berry–Esseen bounds.

We implement the method using [1] and illustrate how it behaves in lowdimensional
settings. Overall, the approach can be seen as a simple and 1 lightweight way to generate perturbations for angle-encoded data, making it useful for applications like explainability (e.g., LIME), robustness analysis, and data augmentation in hybrid quantum-classical workflows.

Please accept or decline the review by 2026-04-29.

You may contact me with any questions about the submission or the review process.

Thank you for considering this request. Your help is much appreciated.

Kind regards,

Editor
