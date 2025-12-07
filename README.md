# CodeAlpha_Basic-chatbot
# Simple Rule-Based Chatbot

def chatbot_reply(user_text):
    user_text = user_text.lower()

    if user_text == "hello":
        return "Hi!"
    elif user_text == "hi":
        return "Hello!"
    elif user_text == "how are you":
        return "I'm fine, thank you!"
    elif user_text == "i am fine":
        return "Nice to hear that!"
    elif user_text == "thanks":
        return "You're welcome!"
    elif user_text == "bye":
        return "Goodbye!"
    else:
        return "Sorry, I don't understand that."

def main():
    print("=== Welcome to Simple Chatbot ===")
    print("Type 'bye' to exit.\n")

    while True:
        user_input = input("You: ")

        reply = chatbot_reply(user_input)
        print("Bot:", reply)

        if user_input.lower() == "bye":
            break

if __name__ == "__main__":
    main()
