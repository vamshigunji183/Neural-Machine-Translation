# language-translation
Neural machine translator for English2German translation.


## Overview
This project is about translation from English to German language. That is accomplished by using TensorFlow library, more specifically it utilizes embedding with attention sequence-to-sequence model.
The python notebook show detailed explanation to the En-De translation.

## Dataset
* OpenSubtitles (movies subtitles)
* http://opus.lingfil.uu.se/OpenSubtitles.php
* for more info take a look at data_utils.py
# Language Translation

Language Translation (NMT).
Example:

Inline-style:
![En-De Translation](https://github.com/vamshigunji183/Neural-Machine-Translation/blob/master/En-De%20Translation/En-De%20Translation.JPG)

## Dependencies

* tensorflow
* nltk
* six

Install missing dependencies with [pip](https://pip.pypa.io/en/stable/)

## Usage

To train model on data and test it to compute the [BLEU score](https://en.wikipedia.org/wiki/BLEU) run this:

``python translate.py source_language target_language`` (i.e. python translate.py fr en for fr->en translation)

## Results

* Translation from French -> English (fr-en dataset)
  * Some success cases

    | French     | English     |
    |----------- |------------ |
    | Bonjour    | Morning     |
    | Au revior  | Good bye    |
    | Merci      | Thanks      |
    | Je m'appelle Dan Ellsey | My name is Dan Ellsey |

  * Some failure cases

    | French | English |
    |--------|-------- |
    | Voici Bill Lange | I am this next woman Bill |
    | La vérité est que le Titanic | Long being why I see special of |
    | Le problème | People |

* Translation from Finnish -> English (fi-en dataset)
  * Some success cases

    | Finnish     | English     |
    |----------- |------------ |
    | Istuntokauden uudelleenavaaminen | Resumption |
    | Hyvaa huomenta  | Good morning |
    | Kiitos      | Thanks  |
    | Nimeni on | My name is |

  * Some failure cases

    | Finnish | English |
    |-------- |-------- |
    | Voin taata täällä | Woman here I here say say say |
    | Haluaisin kuitenkin painottaa | However, it it it stress |
    | sanotun yhteisen maatalouspolitiikan  | s take of of of policy |
