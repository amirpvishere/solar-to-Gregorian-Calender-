# solar-to-Gregorian-Calender-
def date_changing(day, month, year):

    day += 22
    month *= 30
    year *= 365
    x = day + month + year
    y = x + 226665

    if day < 30:
        day -= 30

    month = ((month // 30) + 2 )
    if month > 12:
        month -= 10

    year = y // 365

    print(f'The day of your birth = {year}/{month}/{day}')

day = int(input('Enter the day of your birth: '))

month = int(input('Enter the month of your birth: '))

year = int(input('Enter the year of your birth: '))

date_changing(day,month,year)
