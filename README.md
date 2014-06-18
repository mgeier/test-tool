probably a test tool of some sort
=================================

This is not even work-in-progress, this is potential future work.

A tool for physiological tests with its main focus on psychoacoustics.

Probably written in Python.

Probably having a GUI created with GTK+ and GObject Introspection.
Probably using Glade.

possible example tests
----------------------

* Spatial Release from Masking for Speech

  http://www-users.york.ac.uk/~aqs1/Test4.html

  (probably a version for adults instead of kids)

* McGurk Effect

  http://en.wikipedia.org/wiki/McGurk_effect

  http://www.faculty.ucr.edu/~rosenblu/VSMcGurk.html

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

### BS.1116-1

ITU-R, "ITU-R Recommendation BS.1116-1: Methods for the subjective assessment of
small impairments in audio systems including multichannel sound systems,"
Okt-1997.

http://www.itu.int/rec/R-REC-BS.1116-1-199710-I

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

custom GTK widgets

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

other test software
-------------------

Probably it's not even necessary to create a new framework, there are many out
there ...

* Psychtoolbox-3
** http://psychtoolbox.org/HomePage

> Psychophysics Toolbox Version 3 (PTB-3) is a free set of Matlab and GNU/Octave functions for vision research. It makes it easy to synthesize and show accurately controlled visual and auditory stimuli and interact with the observer.

* "WhisPER" Matlab toolbox
** http://www.ak.tu-berlin.de/menue/digitale_ressourcen/research_tools/whisper_listening_test_toolbox_for_matlab/
** closed source (Matlab p-files)

> WhisPER is a software package for performing experiments in the field of perceptual audio evaluation and psychoacoustic measurement, controlling the interaction with both the subject and the playback environment.

* PsychoPy
** http://www.psychopy.org/

> PsychoPy is an open-source application to allow the presentation of stimuli and collection of data for a wide range of neuroscience, psychology and psychophysics experiments. It’s a free, powerful alternative to Presentation™ or e-Prime™, written in Python (a free alternative to Matlab™ ).

* FLXLab
** http://flxlab.sourceforge.net/

> FLXLab is a program for conducting computer-based experiments in psychology and related fields. It can present stimuli in the form of graphics, text, or sound, and can record responses to those stimuli, either manual (i.e., pressing a key) or verbal.
> FLXLab is currently available for the Windows, OS X, and Linux operating systems.

* MEDS (Music Experiment Development System)
** http://www.schoolofmusic.ucla.edu/pages/Kendall/meds.htm

> The Music Experiment Development System (MEDS) is a Windows based environment for developing and running multimedia perception experiments.

* MLP: a MATLAB toolbox for rapid and reliable auditory threshold
** http://www.psy.unipd.it/~grassi/mlp.html

* APEX 3
** https://gilbert.med.kuleuven.be/web/index.php/Public:Software/APEX

> Apex 3 is a software platform for auditory behavioural and psychophysical experiments. It provides a generic means of setting up experiments without any programming. The supported output devices include sound cards and the Nucleus cochlear implant.

* Experiment Creator
** http://www.psy.mq.edu.au/me2/index.php/site/creator/

* "Interactive Illustrations" in a Java-enabled webbrowser
** http://psych.hanover.edu/JavaTest/Media/Chapter02.html

* PyEPL
** http://pyepl.sourceforge.net/
** Debian package available

> PyEPL (the Python Experiment-Programming Library) is a library for coding psychology experiments in Python. It supports presentation of both visual and auditory stimuli, and supports both manual (keyboard/joystick) and sound (microphone) input as responses.

* Psylab
** http://www.hoertechnik-audiologie.de/psylab/

> "psylab" is a set of scripts, written in Matlab, which are designed to develop and automatically control a large variety of psychoacoustical detection- and discrimination-experiments in a fast and uniform way.

* Lacinato
** http://www.lacinato.com/cm/software/othersoft/abx

<!--
vim:textwidth=80
-->
