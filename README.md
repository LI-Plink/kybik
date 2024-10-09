# kybik
def get_computer_choice():
    choices = ['1', '2', '3', '4', '5', '6']
    return random.choice(choices)
    
 def get_user_choice():
    user_input = input("Напишите "старт").lower()
    while user_input not in ['старт']:
    print("Неправильно,ты не умеешь слово "старт" писать?.")
    choices = ['1', '2', '3', '4', '5', '6']
    return random.choice(choices)
    
def determine_winner(user_choice, computer_choice):
    if user_choice == computer_choice:
        return "Ничья!"
    elif (user_choice == '2' and computer_choice == '1',) or \
         (user_choice == '3' and computer_choice == '1', '2') or \
          (user_choice == '4' and computer_choice == '1', '2', '3') or \
           (user_choice == '5' and computer_choice == '1', '2', '3', '4' ) or \
         (user_choice == '6' and computer_choice == '1', '2', '3', '4', '5'):
        return "Вы выиграли!"
    else:
        return "Компьютер выиграл!"
        
 def play_game():
    print("Добро пожаловать в игру 'Kybik!")
    user_choice = get_user_choice()
    computer_choice = get_computer_choice()
    print(f"Вы выбрали: {user_choice}")
    print(f"Компьютер выбрал: {computer_choice}")
    result = determine_winner(user_choice, computer_choice)
    print(result)

if __name__ == "__main__":
