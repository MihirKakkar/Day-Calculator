def days_difference(day1, day2):
  return day2 - day1 

def get_weekday (day, days_ahead):
  """
  (int, int) -> int

  Return which day of the week it will be days_ahead days
  from day.
  
  day is the current day of the week and is in
  the range 1-7, indicating whether today is Sunday (1),
  Monday (2), ..., Saturday (7).
  
  days_ahead is the number of days after today.

  >>> get_weekday (3, 1)
  4
  >>> get_weekday (6, 1)
  7
  >>> get_weekday (7, 1)
  1
  >>> get_weekday (7, 7)
  7
  >>> get_weekday (1, 0)
  1
  >>> get_weekday (7, 72)
  2
  """
  return (day + days_ahead - 1) % 7 + 1 

def get_birthday_weekday (day, current_day, bday):
  """

  (int, int, int) -> int
  
  Return the day of the week it will be on bday, given that
  the day of the week is day and the day of the year is
  current_day.
  day is the current day of the week and is in the range 1-7,
  indicating whether today is Sunday (1), Monday (2), ..., Saturday (7).
  day and birthday_day are both in the range 1-365.

  >>> get_birthday_weekday (5, 3, 4)
  6
  >>> get_birthday_weekday(5, 3, 116)
  6
  >>> get_birthday_weekday(6, 116, 3)
  5
  """
  days_diff = days_difference(day, bday)
  return get_weekday(current_day, days_diff)

x = get_birthday_weekday(3, 119, 291)
print(x)
