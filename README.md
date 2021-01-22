<pre>
Neon Genesis Evangelion - Typing Project E
English Translation v1.5

Developed by Derek Pascarella (ateam)

Find me on...
 -> SegaXtreme: https://segaxtreme.net/members/ubik.21655/
 -> Dreamcast-Talk: https://www.dreamcast-talk.com/forum/memberlist.php?mode=viewprofile&u=5766
 -> GitHub: https://github.com/DerekPascarella
 -> Twitter: https://twitter.com/DerekPascarella
 -> Reddit: https://www.reddit.com/user/ate4m/


.-----------::[ Patching Instructions ]::-----------
|
| 1) Copy TOSEC-style GDI files (gdi+raws+bins) to the "gdi" folder.
|
| 2) Drag the "gdi" folder onto the "extract_gdi.bat" file.  A new folder called
|    "gdi Extracted" will be created.  This folder contains all of the data files
|    from the game.
|
| 3) Copy all of the files from the "patched_files" folder to the "gdi Extracted"
|    folder, choosing to overwrite existing files when prompted.
|
| 4) Drag the "gdi Extracted" folder onto the "build_gdi.bat" file.  A small black
|    window will open stating that the GDI build process has begun.  Once it has
|    completed, a success message will appear before the window automatically
|    closes after a few seconds.
|
| 5) The GDI files (gdi+raws+bins) in the "gdi" folder are now ready for use.
|
`---------------------------------------------------


.------------::[ v1.5 Release Notes ]::-------------
|
| I am considering this release to be something of a "stop gap" until version 2
| comes along.  With version 1.5, the entire game is now beatable so that
| players can unlock the bonus level and see all content therein.
|
| As explained in the version 1 release notes, the only parts of the game that
| were left unplayable were level 5, level 6, and the bonus level (i.e. level
| 7).  After hours and and hours of effort, I managed to partially
| reverse-engineer the encoding used for the Japanese word bank data for those
| levels.
|
| At present, all rounds these last three levels recycle the same "word" over
| and over again.  That word is "SDFGHJKL", hence why I described my
| reverse-engineering efforts as "partial".  This "word" was chosen for two
| reasons:
|
|   1) It consists of eight characters and thus serves to help increase the
|      player’s total score for each round.
|
|   2) No combination of those letters correlates to and letters-groupings
|      used to generate a Hiragana character.  This is important because the
|      last three levels do not process Roman letters the same way that all
|      previous levels do.  Instead of a 1:1 relationship between what the player
|      types and what appears on-screen, the last three levels convert the Roman
|      letter-groups to Hiragana in order to build the Kanji from each prompt.
|
| A bug fix was also implemented to eliminate all instances of the player being
| required to type the colon character (:), since the character mapping for the
| standard Western Dreamcast QWERTY keyboard does not align with that of the
| Japanese keyboard for that particular character.  Thus, it was impossible for
| the player to actually input that character.
|
| Long term, my goal is to take this translation patch to the next and final
| level by using meaningful word to populate the word banks for level 5, 6, and
| the bonus level (i.e. level 7).  While I’ve made some progress in this
| area, I have not yet arrived at a solution that I am happy with.  That being
| said, I decided to release version 1.5 in order to ensure that all who so
| desire can actually play through and beat the entire game.
|
| Stay tuned!
|
`---------------------------------------------------


.------------::[ v1.0 Release Notes ]::-------------
|
| I’m very proud to release the very first version of my English translation
| patch for "Neon Genesis Evanglion – Typing Project E" for the Sega
| Dreamcast!  Thanks to a very active community, The Dream™ never dies and I
| want to give my most heartfelt "thank you" to each and every person who
| is passionate about Sega’s farewell console.
| 
| In this initial release (version 1), all menus, options, dialog boxes, and
| screens have been fully translated.  Levels 1 through 4 have also been fully
| translated, with the exception of a few short sequences of spoken dialog.
| Levels 5, 6, and the bonus level have only had their menus, dialog boxes and
| screens translated.  However, the levels are not yet playable by a
| non-Japanese speaker.  My goal is to complete a playable version of those
| levels for version 2.  Allow me to elaborate with more detail…
| Part of what made translating this game so attractive to me is the majority
| of the game being QWERTY-keyboard friendly, where an English speaker with
| access to the standard Dreamcast keyboard is able to play and complete each
| level.  Some levels use English words for their word bank, others use the
| Romanji spellings of Japanese words.  In either case, the game is fully
| playable.
| 
| However, the previously mentioned levels (5, 6, and bonus) instead present
| the player with words written in a mixture of Kanji and Katakana/Hiragana.
| The game then expects the player to use the key combinations necessary to
| produce the series of Katana/Hiragana characters that construct one Kanji
| character.  It’s obvious how challenging this is from a translation
| perspective.  There are two approaches to solving this:
|
|   1) Display the Roman alphabet letters that correspond to each Katakana,
|      Hiragana, and Kanji character that the player is asked to type, this way
|      they can easily key in the correct sequence of letters in order to
|      successfully complete the word.  The challenge here is fitting the
|      Roman letters into the space provided on-screen for each character.
|      This is the most straight forward solution as of right now and will
|      likely be polished and implemented in version 2.
|
|   2) Reverse-engineer the game to either:
|        a. Display as many Roman letters as I’d like for each Katakana,
|           Hiragana, or Kanji character.
|        b. Use entirely custom word banks that would allow for me to avoid the
|           Japanese character problem altogether.
|
| At this time of this release, I have not been successful in either of these,
| and of course I welcome any and all contributions from others in the
| community with more experience in this area.
|
| It’s also worth mentioning that level 5 allows the player to "cheat" by
| pressing Enter to display the Katakana/Hiragana equivalent of each Kanji word
| to be typed.  As it is much simpler to fit the two or three Roman letters
| into the space provided for each Katakana/Hiragana character, I initially
| believed that level 5 could be solved in this manner.  However, I quickly
| discovered that by cheating, the player is awarded no points for that
| individual word, thus leaving them with no way to progress.
|
| Lastly, the "WEBPAGE" option on the title screen takes you to a browser that
| displays a website that's stored directly on the disc.  While the browser's
| menu and all of the site's pages are translatable, it's a very low priority
| for me (for obvious reasons).
|
| In summary, this game is extremely playable.  I have had a lot of fun on this
| project and so you can expect a second and final version to be released once
| I overcome the previously mentioned challenges.  I hope you enjoy the game!
|
`---------------------------------------------------


.-----------------::[ Changelog ]::-----------------
|
|  -> 2021-01-22 (v1.5)
|		-Levels 5, 6, and bonus level 7 now beatable (reduced playability).
|		-Fixed colon (:) bug in level 1.
|
|  -> 2021-01-14 (v1.0)
|		-Initial release.
|
`---------------------------------------------------
</pre>
