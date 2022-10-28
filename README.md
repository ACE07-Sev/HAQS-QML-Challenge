# Quantum-Kernel-Esitmation-HAQS
Repository dedicated to the solution proposed by Qualition to HAQS Quantum Hackathon 2022, qBraid's Quantum Machine Learning Challenge.

## Qualition HAQS Team :

John Gardiner (Email : johngoldengardiner@gmail.com, Github username and discord ID: John Gardiner#2496, )

R K Rupesh (Email : rupeshknn@gmail.com, Github username and discord ID: rupeshknn#8939, )

Avhijit Nair (Email : avhijtnair@gmail.com, Github username and discord ID: Avhijit_Nair#5348,  )

Amirali Malekani Nezhad (Email : amiralimlk07@gmail.com, Github username and dicord ID: A.C.E07#8672, https://github.com/ACE07-Sev)

Yousra Bouakba (Email : bouakbayousra@gmail.com, Github username and dicord ID : youyaQ#8253, https://github.com/yousrabou)

Vishal Mandal (Email : vishalmandal091@gmail.com, Github username and dicord ID : Vishal Mandal#7391, https://github.com/Vishal-Mandal

## Model Summary

The challenge was done in two segments,

1) Quantum Variational Classifier : Create a QML pipeline using the variational (parameterized) approach to perform a binary classification. The pipeline starts by generating a random dataset from the gen_binary.py, and in VQC.py we first call the class to generate the random dataset. We then apply a feature map to the initial state to encode the datapoints using angle encoding. Furthermore, we apply the VQC Ansatz (Havlicek et al.) and perform the training process using PennyLane's GradientDescentOptimizer and evaluate the trained model on the test dataset, which yields a %100 (50 out of 50 samples correctly classified) result.

2) Quantum Kernel Estimator : Create a QML pipeline using the kernel estimation approach to perform a binary classification. The pipeline starts by generating a random dataset from the gen_binary.py, and in VQC.py we first call the class to generate the random dataset. We then apply a feature map to the initial state to encode the datapoints using angle encoding. Furthermore, we generate the kernel estimates of the training and test datasets using the circuit from Havlicek et al. and pass the kernel matrices to a classical SVM to perform the optimization, and then evaluate the model against the test dataset.

Both solutions have been uploaded to the src. Kindly read the terms of use under the license.
