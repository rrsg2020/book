# Data Submissions

<p style="text-align:justify;">
Data submissions for the challenge were managed through a dedicated repository on GitHub, accessible at https://github.com/rrsg2020/data_submission. This allowed transparent and open review of the submissions, as well as better standardization of the process. All datasets had to be converted to the NIfTI file format, and images from different TIs needed to be concatenated into the fourth (or “time”) dimension. Magnitude-only datasets required one NIfTI file, while complex datasets required two files (magnitude and phase, or real and imaginary). Additionally, a configuration file containing submission, dataset, and acquisition details (such as data type, submitter name and email, site details, phantom or volunteer details, and imaging protocol details) was required for each submitted dataset to ensure that the information was standardized and easily found. Each submission was reviewed to confirm that guidelines were followed, and then datasets and configuration files were uploaded to OSF.io. A Jupyter Notebook  (Kluyver et al. 2016; Beg et al. 2021) pipeline was used to generate T1 maps at this stage also for quality assurance. Links to the Jupyter Notebook for reproducing the T1 map were shared for each submission using the MyBinder platform, ensuring that computation environments were reproducible without the need for installation of software packages on peoples local computers.
</p>
