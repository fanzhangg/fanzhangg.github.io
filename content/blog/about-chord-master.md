+++
categories = ["development"]
draft = false
image = "img/blog/play_chord.gif"
showonlyimage = false
date = "2020-2-15T21:50:47+05:30"
title = "All About Chord Master"
weight = 1
description = "The vision document for chord master"
+++

![chord](/img/blog/play_chord.gif)

## What are you building? 

Chord Master is a web application that helps musicians find chords and create chord progressions. It helps you find chords that work together.

Chords in the progression are represented by the lead sheet symbol. To build a chord, you can click the + button to add a chord, select the chord type and inversion in the dropdown menu, and choose the root note by clicking its key on the keyboard interface. You can also edit, delete or copy a chord. You can click the play button to listen to the entire chord progression. After finishing the progression, you can download the track as a MIDI file, and use the progression for your song.

### Features:

- Set the chord on one click: Chord Master lets your change the root note, the chord type and the inversion. You can select a root note by pressing a key on the piano keyboard, and switch a chord type or inversion by selecting one in the drop down menu. After each change, the sound of the new chord will be played, so you can compare it with the previous one and see which one fits your song the best.
- Beginner friendly: Don’t know a lot chords? No worry. The app offers 30+ common chord types, categorized by its family. Don’t know the half steps of a chord? No worry. The app will show the notes in the chord by highlighting the keys on the piano, so you can try out the chord on your actual piano right way.  Also, Chord Master shows the standard symbol of the chord. You don’t need to be a music theory master to build the chords with Chord Master!
- Polish your progression: Creating a good progression is not easy, so you can’t build one at once. Chord Master plays the chord you create, so you can know how well your work goes. Meanwhile, you can always edit and delete every chord in the progression.
- Beautiful UI: As you are creating a beautiful progression, we want to make sure the process is enjoyable. Chord Master has a delicate user interface. Our design follows a minimalist principle to avoid distraction. We use bright colors and shadow to highlight the information that is important. Also, every hover and click on a button will give you a response, so you always know what’s going on.

## What problem does it solve?

Chord Master aims to provide an elegant way for musicians to write the chord progressions. To build a chord progression in most music making software, you have to know the half steps of each chord, and click every note manually on the piano roll. However, it is hard to remember the half steps of all chords for a musician who is not familiar with music theory; The effort and time to create a chord might distract the musician in the creation; And it is not easy to change the chord type or inversion of a chord. Therefore, our app wants to create a simple and fluent workflow for musicians to build the chord progression. You can add, edit, delete, or repeat a chord at one click. For each chord, you can easily change the chord type, inversion, or the root note, and visualize the chord via the lead sheet symbol and the highlighted keys on the keys.

## What will it do?

### Create a Chord

A chord is a combination of notes played together to create a rich harmony. A chord is initialized as a C major chord in the app. Each chord is represented by a lead sheet symbol in the button of the chord progression interface. Taking “Cm/E♭” as an example, C is the root note of the chord, “m” indicates it is a minor triad, and “/E♭” shows it is the first inversion.
Change the chord type:  Click the chord type button to open up the dropdown menu. Select the chord family that the chord type is in, and then in the submenu select the chord type. After updating the chord type, the root note will be preserved, and the inversion will be reset to None.

- Change the root note: Each notes in the chord is highlighted on the piano. If the chord is inverted, the original root note will also be highlighted with a gray color. To set a root note, click a key of the root note on the piano, then the highlighted keys, and the chord symbol will be updated, and the sound of the chord will be played.
- Change the inversion: Chord inversion is a modification on a chord that changes which note is the lowest in that chord. Chord Master allows you to select up to third inversion. To change the inversion, select the inversion number on the inversion dropdown menu. To disable the inversion, select “None” in the dropdown menu.

### Build a Chord Progression

- Select a chord: You can select a chord by clicking a button in the chord progression. After a chord is selected, the chord button will be highlighted, and the sound of the chord will be played, and the chord type, inversion, and the notes will be updated accordingly. The chord is then become editable.
- Add a chord: You can add a chord by clicking the + button, then a C major chord will be append after your progression, and the chord will be editable.
- Delete a chord: You can delete a chord by clicking the x button on the left top of each chord.
- Copy a chord to the end: To repeat a chord, you can click the copy button on the bottom right of each chord. The chord will be copied to the end of the progression.
- Play a chord: To play a chord, you can click the play button, and the chord progression will keep playing in a loop. To stop a chord, click the play button again.
- Reset the progression: To clear the progression, you can click the delete button, then a message box will be prompted to ask if you want to reset the progression. If you select yes, the progression will be reseted.
- Save to MIDI file: You can download the progression as a MIDI file by clicking the download button. Then, you can import the track to your favorite music making software. The MIDI file uses the piano as the instrument and the half note by default.

### Who is the end user?

Many musicians might have good sense if  in their mind, but their lack of music theory knowledge may stop them to polish their music. Therefore, our end users are musicians who are looking to create unique chord progressions but may not have a full understanding of music theory.
