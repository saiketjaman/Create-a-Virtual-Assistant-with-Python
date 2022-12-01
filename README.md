# Create-a-Virtual-Assistant-with-Python

## Build an Artificial Assistant
### Python Download 
`https://www.python.org/downloads/`

### Pycharm Download
`https://www.jetbrains.com/pycharm/`


### The packages link used to build it
`https://pypi.org/project/SpeechRecognition/`
`https://pypi.org/project/pyttsx3/`
`https://pypi.org/project/PyAudio/`
`https://pypi.org/project/pywhatkit/`
`https://pypi.org/project/wikipedia/`
`https://pypi.org/project/pyjokes/`
## Installation
### For windows users
(run those in command prompt/cmt/terminal)
For the robot to listen to our voice/speech
`pip install speechRecognition`

To speak out, or text to speech
`pip install pyttsx3`

For advance control on browser
`pip install pywhatkit`

To get wikipedia data
`pip install wikipedia`

To get funny jokes
`pip install pyjokes`

### For linux users
Learn all the above commands on terminal. Make sure to use `pip3`, because in linux `pip` refers for `python2` and `pip3` refers to `python3`.
Install these too - 
`pip3 install pyAudio`

In case any error pops up install this -
`pip3 install portAudio`

### For mac (arm) users
The latest version of MacOS (Ventura) has few issues about pyttsx3 and pyAudio. In order to run this program on Mac successfully, you might need to execute these following commands:
To fix pyttsx3 in Ventura:
```
python -c 'import inspect; from pyttsx3.drivers.nsss import NSSpeechDriver; print(inspect.getsourcefile(NSSpeechDriver))'
```
It should prints something like this:
```
/Users/myuser/virtualenvs/myvenv/lib/python3.10/site-packages/pyttsx3/drivers/nsss.py
```
Use your text editor to find & remove `attr['VoiceAge']`. This should do the trick.

Move on to pyAudio part. 
Manually install portaudio first:

```
git clone https://github.com/PortAudio/portaudio.git
cd portaudio
./configure && make
sudo make install
sudo cp include/pa_mac_core.h /usr/local/include
```

Then
```
pip install pyAudio
```
Should works fine.