1. pip install virtualenv
2. virtualenv Proejct_Name
3. Scripts\activate
4. 建立 requirements.txt 檔案內容
	Django==3.1
	pylint
	pylint-django
	autopep8
5. pip install -r requirements.txt
6. django-admin startproject Hello_world .	# 建立專案
7. python manage.py startapp web	# 建立應用程式
8. code . 開啟VS　Code
9. 設定setting檔案
	{
		"python.pythonPath": "C:\\Users\\User\\AppData\\Local\\Programs\\Python\\Python37\\python.exe",
		"python.linting.pylintPath": "pylint",
		"python.linting.pylintArgs": [
			"--load-plugins", "pylint_django"
		],
		"python.formatting.autopep8Path": "autopep8",
		"python.linting.enabled": true,
		"python.linting.pylintEnabled": true,
		"files.trimTrailingWhitespace": true, // 儲存的時候，會幫你自動過濾多餘的空格
		"files.autoSave": "onFocusChange", // 是否自動儲存檔案
		"[python]":{
			"editor.formatOnType": true,
			"editor.formatOnSave": true,
			"editor.renderIndentGuides": true,
			"editor.insertSpaces": true,
			"editor.detectIndentation": true,
			"editor.tabSize": 4
		},
	}
9. python manage.py runserver