def chatbot_response(user_input):
    user_input = user_input.lower()
    if "hello" in user_input or "hi" in user_input:
        return "Hello! How can I help you today?"
    elif "your name" in user_input:
        return "I'm a simple chatbot created in Python."
    elif "bye" in user_input:
        return "Goodbye! Have a great day."
    else:
        return "Sorry, I didn't understand that. Can you please rephrase?"

def main():
    print("Chatbot: Hello! Type 'bye' to exit.")
    while True:
        user_input = input("You: ")
        response = chatbot_response(user_input)
        print(f"Chatbot: {response}")
        if "bye" in user_input.lower():
            break

if __name__ == "__main__":
    main()
