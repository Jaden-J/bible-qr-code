# bible-qr-code

Have you ever wanted to generate a QR code that opens the Bible to a specific spot?

This simple python script does just that - it uses a [URI intent](https://developer.android.com/reference/android/content/Intent.html) that the
[YouVersion Bible app](https://www.youversion.com/) handles to launch the bible app to the desired location.

## Installation

`pip install pyqrcode pypng argparse`

## Usage

```
$> python bibleqrcode.py --output test.png --chapter 1 --start_verse 1 --end_verse 5 --version KJV Genesis
Generating QR code for intent URI:
https://www.bible.com/en-GB/bible/1/GEN.1.1-5.KJV
Saved test.png
```

![QR Code for above example](test.png)

python bibleqrcode.py --output Pslams23.png --chapter 23 --start_verse 1 --end_verse 6 --version NKJV Psalms
