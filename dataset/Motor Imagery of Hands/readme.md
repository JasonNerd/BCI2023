Dataset Downloads
During the past experiments, we have recorded several datasets under different circumstances. These datasets
can be downloaded for free in the hope that they can help research on signal processing. They have all been
recorded using OpenViBE.

Dataset #1 – Motor Imagery of Hands
Recorded 2008/03, Uploaded 2010/03

This datasets includes 14 records of left and right hand motor imagery.

They include 11 channels : C3, C4, Nz, FC3, FC4, C5, C1, C2, C6, CP3 and CP4.

The channels are recorded in common average mode and Nz can be used as a reference if needed.

The signal is sampled at 512 Hz and was recorded with our Mindmedia NeXus32B amplifier.

Each file consists in 40 trials where the subject was requested to imagine either left or right hand movements (20 each).

The experiment followed the Graz University protocol [as described in “Pfurtscheller, G. & Neuper, C.
Motor Imagery and Direct Brain-Computer Communication. Proceedings of the IEEE, 89, 1123-1134, 2001.”].

The files were recorded on three different days of the same month.

There are 3 CSV files you can download for each record :

signal: contains the raw signal of the experiment.
labels: contains the stimulation codes that happened during the experiment.
spectrum: contains the spectrum of the signal computed on 1 second moving windows.
Please note [that stimulation code (label) meanings](http://openvibe.inria.fr/stimulation-codes/) can be retrieved from dedicated documentation page.

[The spectrum file format](http://openvibe.inria.fr/documentation/unstable/Doc_BoxAlgorithm_CSVFileWriter.html) is documented in the manual of the OpenViBE plugin that created the CSV file..

Finally, there is an OpenViBE scenario which implements the used protocol (see here). Open this scenario and look at “Graz Motor Imagery BCI stimulator” box (a Lua stimulator box) . The exact timing of the protocol is there, together with which stimulation is used to indicate which event (instructions, type of motor imagery, etc.).

The data set has been used in the following paper :

Nicolas Brodu, Fabien Lotte, Anatole Lécuyer. Exploring Two Novel Features for EEG-based Brain-Computer Interfaces: Multifractal Cumulants and Predictive Complexity. Neurocomputing 79: 87-94, 2012. PDF. source code.