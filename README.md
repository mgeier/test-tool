probably a test tool of some sort
=================================

This is not even work-in-progress, this is potential future work.

A tool for physiological tests with its main focus on psychoacoustics.

Probably written in Python.

Probably having a GUI created with GTK+ and GObject Introspection.

Probably using Glade.

... or using [Kivy](https://kivy.org/)?

possible example tests
----------------------

* Spatial Release from Masking for Speech

  * http://www-users.york.ac.uk/~aqs1/Test4.html

    * (probably a version for adults instead of kids)

* McGurk Effect

  * http://en.wikipedia.org/wiki/McGurk_effect

  * http://www.faculty.ucr.edu/~rosenblu/VSMcGurk.html

* non-audio example from "Computational Methods for Psychology and Neuroscience"

  * http://memory.osu.edu/classes/python/assignments/as01_exp.html

possible test methods
---------------------

### Paired Comparisons

...

### A/B/X

http://www.tonmeister.ca/main/textbook/node359.html

### ABC/HR

http://wiki.hydrogenaudio.org/index.php?title=ABC/HR

http://www.audiohq.de/index.php?showtopic=18

### Forced Choice

Literature: Levitt, 1971

http://www.tonmeister.ca/main/textbook/node360.html

http://www.tonmeister.ca/main/textbook/node361.html (2AFC, "reversals", cites Levitt, 1971)

http://www.cis.rit.edu/people/faculty/montag/vandplite/pages/chap_4/ch4p5.html

> The percentage of correct responses (as opposed to the percentage of
> detection) is plotted against stimulus intensity. In the 2AFC procedure, the
> percentages range from 50% to 100% as compared to 0% to 100% in the regular
> MCS psychometric function. That is because as the stimulus becomes too dim to
> detect the subject is guessing [...]. The guessing rate is 50% for two
> alternatives. Threshold values may now be determined from the plot by
> arbitrarily selecting, say 75%, as the threshold value.

> You can use the following equation to adjust for the probability of chance
> guessing:
> $p=\frac{p'-C}{1-C}$
> where
>   p=corrected probability
>   p'=raw probability
>   C=probability of chance success
>   (For 2AFC, C = 0.5, so p'= 0.75 leads to a p = 0.5.)

Ensuring the attention of the subject:

* You can have the subjects press a button that starts a trial.

* "do over" button

> When working close to threshold, it may be frustrating for subjects because
> they may hardly ever really "see" the stimulus. Sometimes trials that are easy
> to detect can be thrown in to relieve this frustration, however these trials
> are not used for analysis.

> Blinks and Inattention: Instead of the "do-over" button, the following
> equation can be used to correct the psychometric function for these trials.
> You must assume a certain rate for missed trials. This rate is usually small,
> for example 1% (rho = 0.01) of the trials are missed.
> $p=\frac{p'-C}{(1-C)(1-\rho)}$
> where p=corrected probability,
>   p'=raw probability,
>   C=probability of chance success,
>   rho=probability of lapses in attention, misdirection of the eye, blinks, etc.

> Feedback: This procedure can be made more "enjoyable" for the subject with the
> addition of feedback. After each trial, you can signal to the subject whether
> they chose the correct alternative. This helps maintain a stable criterion and
> the feedback helps the subject maintain vigilance for the stimuli. Combined
> with self-pacing, the experiment can be quite bearable for the subject.

### Method of Limits

...

### Method of Constant Stimuli

...

### Method of Adjustment

http://www.tonmeister.ca/main/textbook/node362.html

### BS.1116

ITU-R Recommendation BS.1116: Methods for the subjective assessment of small impairments in audio systems

https://www.itu.int/rec/R-REC-BS.1116/en

Similar to A/B/X

http://www.tonmeister.ca/main/textbook/node363.html

> Note that some over-educated people might classify this as a 'double-blind
> triple-stimulus with hidden reference' test.

### Rank Order

http://www.tonmeister.ca/main/textbook/node364.html

### MUSHRA

MUlti Stimulus test with Hidden Reference and Anchors

Developed by the EBU, similar to BS.1116, however, it's designed for bigger
impairments.

http://www.tonmeister.ca/main/textbook/node365.html

### Semantic Differential

...

### Repertory Grid Technique (RGT)

How to get results: factor analysis, principal component analysis,
multidimensional scaling, cluster analysis

Sader, Weber: Psychologie der Persönlichkeit, 1996:

> "Rep-Test" nach Kelly
> Erfassung von "persönlichen Konstrukten"
> in erster Linie als individualdiagnostisches Vorgehen, inedm sie sich auf den
> Einzelnen bezieht und zugleich beschränkt.
> Für systematische Vergleiche zwischen Personen, die gemeinsame Dimensionen
> voraussetzen, und damit für differentialpsychologische Fragestellungen, ist
> der Rep-Test weniger brauchbar. (vgl. Lohaus 1993; Riemann 1991). Seine Stärke
> liegt im Einsatz für den Einzelfall.

http://edutechwiki.unige.ch/en/Repertory_grid_technique

http://www.tonmeister.ca/main/textbook/node367.html

http://www.pcp-net.de/papers/ueberbli.htm

### Quantitative Descriptive Analysis

http://www.tonmeister.ca/main/textbook/node368.html

### QUEST+

https://jov.arvojournals.org/article.aspx?articleid=2611972

https://github.com/hoechenberger/questplus

some general topics
-------------------

http://www.tonmeister.ca/main/textbook/node348.html

http://irtel.uni-mannheim.de/lehre/seminar-psychophysik/artikel/PsychometrischeFunktion.htm

* direct scaling vs. indirect scaling
* hedonic vs. non-hedonic also called pragmatic
* sensation vs. perception

### Subjective vs. Objective

Fog, C. L. and Pedersen, T. H. (1999).
Tools for product optimisation.
In Human Centered Processes, Brest, France.

see  
https://web.archive.org/web/20110828134303/  
http://www.tonmeister.ca/main/textbook/node350.html  
http://nwavguy.blogspot.de/2011/05/subjective-vs-objective-debate.html

Distinction between and *epistemic* and an *ontological* sense of
subjective/objective in: John R. Searle, The Construction of Social Reality,
Simon and Schuster 1995 (see page 8).
https://books.google.de/books?id=zrLQwJCcoOsC

### Randomization

to avoid *order effects* ...

### Test Duration

ITU-R BS.1116-1 (4.2):

> A grading session should not last for more than 20-30 min, although the
> self-paced character of trials advocated here will introduce uncontrolled
> variability among subjects. Experience suggests that no more than 10 to 15
> trials per session should be scheduled to achieve the desired session length.
> Subject fatigue may become a major factor which would seriously interfere with
> the validity of judgements. To avoid this, rest periods equal to a duration no
> less than the session length should be scheduled between successive sessions
> for each subject.

### Stimulus Duration/Switching

ITU-R BS.1116-1 (4.2):

> Since long- and medium-term aural memory is unreliable, the test procedure
> should rely exclusively on short-term memory. This is best done if a
> near-instantaneous switching (see Note 1) method is used in conjunction with a
> triple stimulus system as described in Appendix 3. Such switching demands
> close time alignment among the stimuli.

> NOTE 1 – Exact instantaneous switching can produce artefacts if the waveforms
> of successive stimuli are not identical. For example, near-instantaneous
> switching with about 40 ms in total for fade-down/change-over/fade-up is
> preferred.

ITU-R BS.1116-1 (section 6):

> Audio excerpts will be typically 10 to 25 s long.

### Audible/Visible Distractions

ITU-R BS.1116-1 (4.2):

> Preferably, the subject should be able to switch between stimuli without
> visual guidance, so that, if the subject wishes, the eyes might remain closed
> for better concentration under conditions of minimal distraction. There should
> be no audible artefacts (e.g. “clicks”) of the switching system, since such
> artefacts can seriously interfere with the assessment process.

### Test Instructions

Each subject should get (ideally the same) oral *and* written instructions.

TODO: examples

### Pre-screening of subjects

e.g. based on audiometric tests or based on the training phase

*All* judgements from a particular subject must be omitted.

Rejection technique/criterion must be clearly described.

### Post-screening

Two classes according to ITU-R BS.1116-1 (section 3.2.2):

* the first is based on inconsistencies compared with the mean result (never
  justifiable)

* the second relies on the ability of the subject to make correct
  identifications (automatically available)

  * t-test

statistics
----------

Bech, S. and Zacharov, N. (2006).
Perceptual Audio Evaluation - Theory, Method and Application.
John Wiley & Sons.

Entscheidungsbaum: Die Auswahl statistischer Tests und Maße:
http://www.psych.uni-halle.de/abteilungen/allgemeine_psychologie/mitarbeiter/blankenberger/entscheidungsbaum/

### Test for ANOVA

suggested: Shapiro-Wilks-, Anderson-Darling- and Cramér-von-Mises-Test

not suggested, but very common: Kolmogorov-Smirnov-Test, Lilliefors, $\chi^2$-Test (Chi-square Test) for distribution

Test homogenity of variance: Bartlett-Test, Levene-Test

GUI stuff
---------

http://python-gtk-3-tutorial.readthedocs.org/

custom GTK widgets

http://stackoverflow.com/a/20595547/500098

http://zetcode.com/gui/pygtk/customwidget/

http://library.gnome.org/devel/gladeui/unstable/pythonsupport.html

http://unpythonic.blogspot.com/2007/03/custom-pygtk-widgets-in-glade3.html
http://unpythonic.blogspot.com/2007/03/custom-pygtk-widgets-in-glade3-part-2.html

(http://www.pygtk.org/articles/custom-widgets-glade/Custom_PyGTK_Widgets_in_Glade3-part-2.html)
Edit
Plotting with Python

matplotlib: http://matplotlib.sourceforge.net/

Tutorials:
http://www.serpia.org/blog/2007/nov/03/matplotlib-and-pygtk-app/
http://www.freesbi.ch/en/python-gtk-plot

Scale example

https://developer.gnome.org/gnome-devel-demos/stable/scale.py.html.en

other test software
-------------------

Probably it's not even necessary to create a new framework, there are many out
there (see [Wikipedia](https://en.wikipedia.org/wiki/Comparison_of_behavioral_experiment_software)) ...

* Psychtoolbox-3
  * http://psychtoolbox.org/HomePage

> Psychophysics Toolbox Version 3 (PTB-3) is a free set of Matlab and GNU/Octave functions for vision research. It makes it easy to synthesize and show accurately controlled visual and auditory stimuli and interact with the observer.

* "WhisPER" Matlab toolbox
  * http://www.ak.tu-berlin.de/menue/digitale_ressourcen/research_tools/whisper_listening_test_toolbox_for_matlab/
  * closed source (Matlab p-files)

> WhisPER is a software package for performing experiments in the field of perceptual audio evaluation and psychoacoustic measurement, controlling the interaction with both the subject and the playback environment.

* PsychoPy
  * http://www.psychopy.org/
  * buttons, sliders, etc.: qLib
    * http://psych.colorado.edu/wiki/doku.php?id=labs:clipr:qlib

> PsychoPy is an open-source application to allow the presentation of stimuli and collection of data for a wide range of neuroscience, psychology and psychophysics experiments. It’s a free, powerful alternative to Presentation™ or e-Prime™, written in Python (a free alternative to Matlab™ ).

* FLXLab
  * http://flxlab.sourceforge.net/

> FLXLab is a program for conducting computer-based experiments in psychology and related fields. It can present stimuli in the form of graphics, text, or sound, and can record responses to those stimuli, either manual (i.e., pressing a key) or verbal.
> FLXLab is currently available for the Windows, OS X, and Linux operating systems.

* MEDS (Music Experiment Development System)
  * http://www.schoolofmusic.ucla.edu/pages/Kendall/meds.htm

> The Music Experiment Development System (MEDS) is a Windows based environment for developing and running multimedia perception experiments.

* MLP: a MATLAB toolbox for rapid and reliable auditory threshold
  * http://www.psy.unipd.it/~grassi/mlp.html

* APEX 3
  * https://gilbert.med.kuleuven.be/web/index.php/Public:Software/APEX

> Apex 3 is a software platform for auditory behavioural and psychophysical experiments. It provides a generic means of setting up experiments without any programming. The supported output devices include sound cards and the Nucleus cochlear implant.

* Experiment Creator
  * http://www.psy.mq.edu.au/me2/index.php/site/creator/

* "Interactive Illustrations" in a Java-enabled webbrowser
  * http://psych.hanover.edu/JavaTest/Media/Chapter02.html

* PyEPL
  * http://pyepl.sourceforge.net/
  * Debian package available

> PyEPL (the Python Experiment-Programming Library) is a library for coding psychology experiments in Python. It supports presentation of both visual and auditory stimuli, and supports both manual (keyboard/joystick) and sound (microphone) input as responses.

* Psylab
  * http://www.hoertechnik-audiologie.de/psylab/

> "psylab" is a set of scripts, written in Matlab, which are designed to develop and automatically control a large variety of psychoacoustical detection- and discrimination-experiments in a fast and uniform way.

* Lacinato
  * http://www.lacinato.com/cm/software/othersoft/abx

* ExpSuite
  * https://www.kfs.oeaw.ac.at/index.php?option=com_content&view=article&id=353&Itemid=521&lang=en
  * http://sourceforge.net/projects/expsuite/

* PyExperimentSuite
  * http://www.rueckstiess.net/projects/expsuite/
  * https://github.com/rueckstiess/expsuite

* GuineaPig (2)
  * Hynninen, Jussi, and Nick Zacharov. "GuineaPig - A Generic Subjective Test System for Multichannel Audio." Audio Engineering Society, 1999. http://www.aes.org/e-lib/browse.cfm?elib=8309.
  * http://legacy.spa.aalto.fi/projects/GuineaPig2/
  * http://research.spa.aalto.fi/publications/theses/hynninen_mst.pdf

* scale: Setup, Conduction and Analysis of Listening Experiments
  * http://www.audiogroup.web.fh-koeln.de/scale.html
  * for Matlab, closed source, precompiled for Windows

* Web Audio Evaluation Tool
  * https://code.soundsoftware.ac.uk/projects/webaudioevaluationtool/
  * Nicholas Jillings, Brecht De Man, David Moffat and Joshua D. Reiss, "Web
    Audio Evaluation Tool: A Browser-Based Listening Test Environment," 12th
    Sound and Music Computing Conference, July 2015.
    [PDF](http://www.brechtdeman.com/publications/smc10.pdf)

> A tool based on the HTML5 web audio API to perform audio evaluation tests on remote machines over the web.

* APE Perceptual Evaluation
  * https://code.soundsoftware.ac.uk/projects/ape
  * B. De Man and Joshua D. Reiss,
    APE: Audio Perceptual Evaluation toolbox for MATLAB,
    136th Convention of the Audio Engineering Society, 2014.
    [PDF](http://brechtdeman.com/publications/aes136.pdf)

> Open perceptual evaluation toolbox for MATLAB.

* OpenSesame
  * http://osdoc.cogsci.nl/
  * GPL

> OpenSesame is a graphical, open-source experiment builder for the social sciences. It sports a modern and intuitive user interface that allows you to build complex experiments with a minimum of effort. With OpenSesame you can create a wide range of experiments. The plug-in framework and Python scripting allow you to incorporate external devices, such as eye trackers, response boxes, and parallel port devices, into your experiment.

* Expyriment
  * http://www.expyriment.org/

> Expyriment is an open-source and platform independent light-weight Python library for designing and conducting timing-critical behavioural and neuroimaging experiments. The major goal is to provide a well-structured Python library for a script-based experiment development with a high priority on the readability of the resulting programme code.

* RateIt: An Open-Source Tool For Performing MUSHRA Tests
  * http://rateit.sourceforge.net/

> RateIt is a GUI tool for performing subjective testing of audio samples based on the MUltiple Stimuli with Hidden Reference and Anchor (MUSHRA) methodology as specified in ITU-R recommendation BS.1534-1. RateIt is dual-licensed under the General Public License (GPL) and the Mozilla Public License (MPL) version 1.1.
>
> RateIt is written in C using libglade, which means that the user interface is very easy to customise. It currently uses sox for playback but support for libsndfile is planned (patches welcome).

* PEBL: The Psychology Experiment Building Language
  * http://pebl.sourceforge.net/
  * GPL

> * Free psychology software for creating experiments,
> * Allows you to design your own experiments or use ready-made ones
> * Lets you exchange experiments freely without license or charge

* testable (commercial)
  * http://www.testable.org/

* State Machine Interface Library for Experiments
  * https://github.com/compmem/smile/
  * "kivy" branch: https://github.com/compmem/smile/tree/kivy
  * probably the predecessor of https://github.com/compmem/psyqt/?

* BeaqleJS (browser based evaluation of audio quality and comparative listening environment)
  * http://hsu-ant.github.io/beaqlejs/
  * https://github.com/HSU-ANT/beaqlejs
  * GPL

> provides a framework to create browser based listening tests and is purely based on open web standards like HTML5 and Javascript.

* https://github.com/maxgiller/listening-test

* Vision Egg
  * https://visionegg.readthedocs.io/

> The Vision Egg is a powerful, flexible, and free way to produce stimuli for vision research experiments.

* HULTI-GEN
  * https://www.hud.ac.uk/research/researchcentres/mtprg/projects/apl/resources/hulti-gen/
  * http://eprints.hud.ac.uk/24809/

> ... HULTI-GEN (Huddersfield Universal Listening Test Interface Generator), a
Cycling ‘74 Max-based tool. HULTI-GEN is a user-customisable environment, which takes user-defined parameters (e.g. the number of trials, stimuli and scale settings) and automatically constructs an interface for comparing auditory stimuli, whilst also randomising the stimuli and trial order.

* Web Audio Evaluation Tool (WAET)
  * https://github.com/BrechtDeMan/WebAudioEvaluationTool
  * Web Audio Evaluation Tool: A framework for subjective assessment of audio,
    https://smartech.gatech.edu/handle/1853/54595

> A tool based on the HTML5 Web Audio API to perform perceptual audio evaluation tests locally or on remote machines over the web.

* expyfun
  * https://github.com/LABSN/expyfun

> This package is designed for audio-visual experiments with precise timing, and includes functionality for Eyelink control. This package is designed with the purpose that it be used by LABS^N at the University of Washington. It is not designed for public use.

* webMUSHRA
  * https://github.com/audiolabs/webMUSHRA
  * https://audiolabs.github.io/webMUSHRA

> a MUSHRA compliant web audio API based experiment software

* earyx
  * https://github.com/TGM-Oldenburg/earyx
  * http://earyx.readthedocs.io/

> earyx is a framework for developing and running psychoacoustic experiments. It is inspired by Psylab a Matlab implementation written by Martin Hansen.

* Listen
  * https://github.com/deeuu/listen
  * https://deeuu.github.io/listen/

> Run listening tests in the browser locally or via GitHub pages

* jsPsych
  * https://www.jspsych.org/
  * https://github.com/jspsych/jsPsych/

> A JavaScript library for creating and running behavioral experiments in a web browser

<!--
vim:textwidth=80
-->
