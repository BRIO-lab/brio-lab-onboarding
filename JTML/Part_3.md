[Previous](https://github.com/BRIO-lab/brio-lab-onboarding/blob/main/JTML/Part_2.md) | [Next](https://github.com/BRIO-lab/brio-lab-onboarding/blob/main/JTML/Part_4.md)

# JTML Part 3: Model-Image Registration

Model image registration is the process of lining up a 3D model to a 2D image that contains pixels representing that model. The goal of this process is to extract out the pose of an object (6 degrees of freedom) from a 2-dimensional image. Similar to a system of equations, having only a 2D image is insufficient to estimate the pose of an object. We need some extra information, such as 3D model information, camera properties (or x-ray detector properties), and some clever data storage techniques.

The following papers are examples of different types of model-image registration problems that have been used for generating kinematics of knee replacements. Please read them and ask any questions that you might have.

[Banks and Hodge - 1996 - Accurate measurement of three-dimensional knee replacement kinematics using single-plane fluoroscopy](https://www.dropbox.com/s/q01w502tf7pv9dj/Banks%201996%20-%20Accurate%20Measurement%20of%20Three-Dimensional%20Knee%20Replacement%20Kinematics%20Using%20Single-Plane%20Fluoroscopy.pdf?dl=0)

[Zuffi et al - 1999 - A model-based method for the reconstruction of total knee replacement kinematics](https://www.dropbox.com/s/122p4jsizj8q3w7/Zuffi%20-%20Single%20plane%20with%20distance%20maps%20-%20IEEE%20TMI%201999.pdf?dl=0)

[Mahfouz et al - 2003 - A robust method for registration of three-dimensional knee implant models to two-dimensional fluoroscopy images](https://www.dropbox.com/s/dst3nnjxpcvkhvn/Mahfouz%202003%20-%20A%20Robust%20Method%20for%20Registration%20ofThree-Dimensional%20Knee%20Implant%20Models%20toTwo-Dimensional%20Fluoroscopy%20Images.pdf?dl=0)

The newest development that our lab has created is utilizing a form of Lipschitzian optimization without the need of a Lipschitz constant (don't worry about what this means just yet) in the form of DIviding RECTangles (DIRECT). The following paper outlines this development.

[Flood and Banks - 2018 - Automated registration of 3-D knee implant models to fluoroscopic images using lipschitzian optimization](https://www.dropbox.com/s/m96mfwl7c8l4x35/Flood%202018%20-%20Automated%20Registraion%20of%203d%20knee%20implants%20lipschitzian.pdf?dl=0)


## Limitations of These Experiments and What We Hope To Accomplish


The goal of this research project is to be able to perform these types of measurements fully autonomously. One of the main limitations and drawbacks from each of these methods is that they all rely on some form of human supervision, either to generate an initial guess (Flood and Banks) or to monitor the progress and ensure that the system does not fall into a local minimum (Mahfouz et al.). Another limitation from these experiments is that they require a decent segmentation of the implant of interest (Banks and Hodge), limiting use in cases with implant occlusion.

We hope to solve all of these problems (and more) by integrating machine learning and neural networks.



[Previous](https://github.com/BRIO-lab/brio-lab-onboarding/blob/main/JTML/Part_2.md) | [Next](https://github.com/BRIO-lab/brio-lab-onboarding/blob/main/JTML/Part_4.md)