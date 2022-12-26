# chrome-selenium-docker
Example python code:
```
from selenium import webdriver
from selenium.webdriver.chrome.options import Options

options = Options()
options.add_argument(profile)
options.add_argument("start-maximized")
options.add_argument('--no-sandbox')
options.add_argument('--window-size=1920,1080')
options.add_argument('--disable-gpu')
options.add_argument("--headless")
options.add_argument("--disable-dev-shm-usage")
options.add_experimental_option("excludeSwitches", ["enable-automation"])
options.add_experimental_option('useAutomationExtension', False)
driver = webdriver.Chrome(chrome_options=options)
driver.get('https://google.com/')
print(driver.title)
```
