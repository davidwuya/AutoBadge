# AutoBadge
Beat formalism and bureaucracy by automatically completes UCSB's pointless screening survey.

## Disclaimer
I, the author of this code, assumes no responsibility for any and all potential consequence for any user. This is a fun side project that I coded in less than an hour to experiment with Selenium. This applet stores your ID and password in PLAIN TEXT, so this will compromise your information security if the computer you're running it on is not safe. You should not use this tool if you're experiencing any COVID-19 symptoms, by using this tool, you are attesting that you do not have any symptoms or experiences that are listed on the UCSB COVID Daily Screening Survey.

## Prerequisite
Python 3+\
Selenium\
Selenium chrome driver\
pyvirtualdisplay for headless usage

```bash
pip3 install selenium
brew install chromedriver #macOS install using Homebrew
#Google for install instructions for other OS
```

## Usage
Have your phone ready for two-factor authentication (by default, it will wait for 60 seconds for 2FA to be completed). Replace the sample username and password at the top of the code. Run the script with command shell or your IDE of choice, filling in the credentials in the top of the code (your UCSB Net ID and password). Check your email after the script's finish running to receive the green badge.
```python
python3 AutoBadge.py
```
You could also do this headlessly (say, on a EC2 Instance) by using pyvirtualdisplay. Uncomment a few lines and you're rocking (after you installed the prerequisites, and Chrome/Chrome Driver).

## To-do
- Automate 2FA
- Grab the badge from portal and save it somewhere
