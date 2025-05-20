from datetime import datetime


class Person:
    def __init__(self, name):
        self.name = name

    def status(self, year_of_birth):
        current_year = datetime.now().year
        if current_year - year_of_birth >= 18:
            print('Вы можете смотреть все страницы сайта')
        else:
            print('Часть страниц вам не доступна')


student = Person('Антон')
# Тесты
student.status(2020)# My-first-repository
