# voice-bot
Trying to make a simple voice bot on Python

## Dependencies Required
  * pyaudio
  * pyttsx3
  * pygame
  * pyowm
  * SpeechRecognition
  * wikipedia
  * pyaudio

Please install these dependencies before running the code.

Note - Works fine on my Windows 10 installation but does not work on my Ubuntu 18.04 installation.

Error on Ubuntu machine:
Traceback (most recent call last):
  File "voice_bot.py", line 13, in <module>
    engine = pyttsx3.init()
  File "/usr/local/lib/python2.7/dist-packages/pyttsx3/__init__.py", line 46, in init
    eng = Engine(driverName, debug)
  File "/usr/local/lib/python2.7/dist-packages/pyttsx3/engine.py", line 52, in __init__
    self.proxy = driver.DriverProxy(weakref.proxy(self), driverName, debug)
  File "/usr/local/lib/python2.7/dist-packages/pyttsx3/driver.py", line 75, in __init__
    self._module = importlib.import_module(name)
  File "/usr/lib/python2.7/importlib/__init__.py", line 37, in import_module
    __import__(name)
  File "/usr/local/lib/python2.7/dist-packages/pyttsx3/drivers/espeak.py", line 5, in <module>
    from . import _espeak, toUtf8, fromUtf8
  File "/usr/local/lib/python2.7/dist-packages/pyttsx3/drivers/_espeak.py", line 18, in <module>
    dll = cdll.LoadLibrary('libespeak.so.1')
  File "/usr/lib/python2.7/ctypes/__init__.py", line 444, in LoadLibrary
    return self._dlltype(name)
  File "/usr/lib/python2.7/ctypes/__init__.py", line 366, in __init__
    self._handle = _dlopen(self._name, mode)
OSError: libespeak.so.1: cannot open shared object file: No such file or directory
