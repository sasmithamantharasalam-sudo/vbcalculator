# vbcalculator
# Voice-Based Calculator 🎙️➗

A single-screen Android app, built with **MIT App Inventor**, that lets you speak a simple arithmetic question out loud and get the answer back — both on screen and read aloud.

## How it works

1. Tap **"ASK A QUESTION"**
2. Speak a two-operand arithmetic question, e.g. *"5 + 3"*
3. The app transcribes your speech and shows it under **QUESTION**
4. It parses the number, operator, and number, calculates the result, and shows it under **ANSWER**
5. It speaks the result back: *"The answer is: 8"*

## Features

- 🎤 Voice input via device microphone (`SpeechRecognizer`)
- 🔊 Voice output via text-to-speech (`TextToSpeech`)
- ➕➖✖️➗ Supports `+`, `-`, `x`, `/`
- 🖥️ Simple single-screen UI — no typing needed

## Tech Stack

- **Platform:** MIT App Inventor (block-based, no native code)
- **Components:** `SpeechRecognizer1`, `TextToSpeech1`, `Button1`, `Label2` (question), `Label5` (answer)
- **Permissions:** `RECORD_AUDIO`, `INTERNET` (cloud-based speech recognition)

## Example

| You say      | Question shown | Answer   |
|--------------|-----------------|----------|
| "5 + 3"      | 5 + 3           | 8        |
| "10 - 4"     | 10 - 4          | 6        |
| "6 x 7"      | 6 x 7           | 42       |
| "20 / 5"     | 20 / 5          | 4        |

## Screenshot



![App Screenshot](Screenshot%20(206)

.png)

*The app in action — showing the recognized question and computed answer.*

## Limitations (v1.0)

- Only recognizes questions in the exact form `number operator number` (e.g. "5 + 3", not "five plus three")
- Only 4 operators supported: `+`, `-`, `x`, `/`
- No divide-by-zero guard
- No calculation history — resets each session
- Requires an internet connection (speech recognition is cloud-based)

## Future Improvements

- Input validation for numbers/operators
- Divide-by-zero handling
- Error message + retry prompt for unrecognized speech
- Support for spoken words like "plus", "minus"

---
*Built as a mini project — SRS follows IEEE Std 830-1998 conventions.*
