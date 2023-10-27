from flask import *
import os

companyDb = {
    "Отдел разработки":{
        "Главный разработчик":"Федоров Руслан",
        "Младший разработчик":"Иванова Ирина",
        "Тестировщик":"Романов Петр"
    },
    "Бухгалтерия":{
        "Старший бухгалтер":"Петров Иван",
        "Бухгалтер":"Антонова Ольга"
    }
}

def index():
    return render_template('index.html', db = companyDb)

folder = os.getcwd()
app = Flask(__name__, template_folder=folder, static_folder=folder) 

app.add_url_rule('/', 'index', index)

if __name__ == "__main__":
    app.run()
