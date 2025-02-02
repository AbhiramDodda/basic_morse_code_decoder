morse_code_dict = {
    '.-': 'A', '-...': 'B', '-.-.': 'C', '-..': 'D', '.': 'E',
    '..-.': 'F', '--.': 'G', '....': 'H', '..': 'I', '.---': 'J',
    '-.-': 'K', '.-..': 'L', '--': 'M', '-.': 'N', '---': 'O',
    '.--.': 'P', '--.-': 'Q', '.-.': 'R', '...': 'S', '-': 'T',
    '..-': 'U', '...-': 'V', '.--': 'W', '-..-': 'X', '-.--': 'Y', '--..': 'Z',
    '-----': '0', '.----': '1', '..---': '2', '...--': '3', '....-': '4',
    '.....': '5', '-....': '6', '--...': '7', '---..': '8', '----.': '9'
}

def decode_morse(morse_code):
    words = morse_code.strip().split('   ')
    decoded_message = ''
    for word in words:
        letters = word.split(' ')
        for letter in letters:
            decoded_message += morse_code_dict.get(letter, '?')
        decoded_message += ' '
    return decoded_message.strip()

if __name__ == "__main__":
    print("Morse Code Decoder")
    print("Enter Morse code with spaces between letters and three spaces between words.")
    print("Type 'exit' to quit.")
    
    while True:
        user_input = input("\nEnter Morse code: ")
        if user_input.lower() == 'exit':
            print("Exiting Morse Code Decoder. Goodbye!")
            break
        decoded_message = decode_morse(user_input)
        print(f"Decoded Message: {decoded_message}")
