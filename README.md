# Chatbot-with-rule-based-responses
codsoft
def chatbot_response(user_input):
    responses = {
        "hello": "Hi there! How can I help?",
        "bye": "Goodbye! Have a great day.",
        "how are you": "I'm just a bot, but I'm doing well!"
    }
    return responses.get(user_input.lower(), "I'm sorry, I don't understand.")
    
while True:
    user_input = input("You: ")
    if user_input.lower() == "exit":
        break
    print("Bot:", chatbot_response(user_input))

Output:
You: hi
Bot: I'm not sure how to respond to that.
You: hello
Bot: Hi! How can I help you?
You: bye
Bot: Goodbye! Have a nice day!
You: how are you
Bot: I'm just a bot, but I'm doing great!
