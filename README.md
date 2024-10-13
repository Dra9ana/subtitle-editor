
# OBJECT-ORIENTED PROGRAMMING - Homework Assignment No. 1

## Functional Specification  
Implemented a static library (.lib) of classes for processing movie subtitles in C++.


## Class Specification: SubtitleEditor  
The `SubtitleEditor` class is designed for loading, processing, and saving a sequence of subtitles. Key features include:

- **Proper Object Creation and Destruction:** Implemented proper creation and destruction of `SubtitleEditor` class objects.
  
- **Subtitle Format:** The system supports a specific subtitle format that includes:
  - A numerical identifier for each subtitle in the sequence.
  - Timing information in the format: hours:minutes:seconds,milliseconds.
  - Stylized text within the subtitles, using special markers for bold, italic, and underline styles, while ensuring no nested styles are allowed.
  - Empty lines at the end of each subtitle and sequence.

- **Loading and Saving Subtitles:** 
  - Implemented `int SubtitleEditor::loadSubtitles(string subtitles);` to load subtitles, returning -1 for success or the line number of a syntax error.
  - Implemented `string SubtitleEditor::saveSubtitles();` to return the sequence of subtitles in the specified format.

- **Selection and Processing of Subtitles:** 
  - Implemented methods for selecting, deselecting, and processing subtitle selections.
  - Functions to add to the selection, remove styles, and adjust timing (shift forward/backward).

- **Subtitle Styling:** Implemented functions to apply and remove bold, italic, and underline styles for selected text in the subtitles.

- **Error Resolution:** 
  - Implemented functions to fix long lines and excessive durations in subtitles, ensuring proper formatting and distribution.

- **Undo Functionality:** Added the ability to undo the last change made to the subtitle sequence.

## Technical Requirements:  
- Utilized only the `string` data type from the Standard Library; all other data structures were implemented from scratch without using the Standard Template Library (STL), including lists and other data structures.
- Managed dynamic memory properly throughout the implementation.
- Organized code into appropriate `.h` and `.cpp` files to maintain project structure.

