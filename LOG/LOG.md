# Project: Project 7b - Neural Representation of Massive 3D Data
- Supervisor: Jens Sjölund <jens.sjolund@it.uu.se>
- Group Members:
    - Aoping Lyu <aoping.lyu.6830@student.uu.se>
    - Jinglin Gao <jinglin.gao.1941@student.uu.se>



## Week 1 Summary (10/30 - 11/5)



### Tuesday (10/31)
- Meeting with the supervisor.

### Thursday (11/2)
- Meeting with the supervisor and the project course convenor.
- Finished downloading the raw files.

### Friday (11/3)
- Identified two possible related open-source libraries:
    - [SlicerMorph](https://github.com/SlicerMorph/SlicerMorph): An extension for importing microCT data and conducting 3D morphometrics in Slicer.
    - [Draco](https://github.com/google/draco): A library for compressing and decompressing 3D geometric meshes and point clouds.


## Week 2 Summary (11/6 - 11/12)

### Read papers
- Neural Fields in Visual Computing and Beyond (For general concepts gaining)
    - Investigate general concepts of neural fields and methods exists for 3D image reconstruction
    - Neural fields can parameterize density domain by directly predicts the density value at a 3D spatial coordinate, and the process is supervised by mapping its output to the senosr domain via Radon(CT) or Fourier(MRI) transform.
- NeRP: Implicit Neural Representation Learning with Prior Embedding for Sparsely Sampled Image Reconstruction
    - MRI reconstruction (Fourier transform)
    - CT reconstruction (Radon transform)
- CoIL: Coordinate-based Internal Learning for Imaging Inverse Problems
    - CT reconstruction
    - Training MLP on the coordinate-response pairs to build a full measurement neural representation.
    

### Work for next week
- Done some literature review
- Start trying out the representation methods

### Proposed Pipeline:
- Data Pre-procesessing and Representation
- Construct Neural Network Model
- Training the Model
- Encoding and Decoding
- Optimization and Evaluation
- Visualisation and Interaction
- Downstream Application




## Week 3 Summary (11/13 - 11/19)

### Key Paper Review
#### SCI: A Spectrum Concentrated Implicit Neural Compression for Biomedical Data

- Paper link: https://doi.org/10.48550/arXiv.2209.15180
    - Focuses on compressing biomedical data, distinct from natural images/videos.
    - Introduces Spectrum Concentrated Implicit neural compression (SCI) based on Implicit Neural Representation (INR).
    - Adapts data into blocks matching INR’s concentrated spectrum envelope.
    - Utilizes a funnel-shaped network for efficient data representation.
    - Implements a parameter allocation strategy for accurate data representation.

    

### Work for next week
- Reproduce the implicit neural compression method using in the found paper.
- Apply it to the 3D data we have.

### Proposed Pipeline:
- Data Pre-procesessing and Representation
- Construct Neural Network Model
- Training the Model
- Encoding and Decoding
- Optimization and Evaluation
- Visualisation and Interaction
- Downstream Application