# hunspell_ja_JP

Hunspell morphology dictionary for Japanese used in GoldenDict.

Hunspell dictionary to deinflect all Japanese conjugated verbs to the
dictionary form and suggest correct spelling.

The conversion method is based on the next point to the word stem. For instance
when faced with 書かない, you have to look up 書か. The advantage of this
method is that it supports any kind of possible conjugation (slang, archaism,
dialect,...) given that the stem word is included in the .dic file. For this
purpose I have compiled every applicable entry from
広辞苑、大辞林、デジタル大辞泉、日本国語大辞典、旺文社国語辞典、明鏡国語辞典、新明解国語辞典
and JMDict. This also allows for spelling suggestions when a word is not found.

This makes for a yomichan like experience when coupled with the scan popup
function. (Preferences > Scan Popup)

## Installation

1. Install GoldenDict.
   Use [xiaoyifang's webengine fork](https://github.com/xiaoyifang/goldendict)
   if you plan to use epwing dictionaries, it includes a fix.
   See https://github.com/goldendict/goldendict/issues/1551)
3. Download both ja_JP.aff and ja_JP.dic.
4. Place both files in a folder.
5. Open GoldenDict, navigate to Edit > Dictionaries > Morphology.
6. Change the directory path to the one you have downloaded the files to.
2. Quit GoldenDict and reopen it to let it automatically detect the added Japanese morphology.
4. Go to the Dictionary setting in the app, and enable the added morphology.
   Also add it to your Dict groups if you want.
5. It should be working now.

# Examples:

#### De-Inflection:

https://user-images.githubusercontent.com/34507493/187703021-066b8d99-a181-45cf-bc4f-f3d05f3d63c0.mp4

#### Spelling Suggestion:

![image](https://user-images.githubusercontent.com/34507493/187703775-98b4f3d0-0505-442b-92ed-e09c4b28ac27.png)

## Acknowledgments

To create this repository I merged together these two repositories:

* https://github.com/MrCorn0-0/hunspell_ja_JP/
* https://github.com/epistularum/hunspell-ja-deinflection

Then sorted the dictionary with `sort -u`.
