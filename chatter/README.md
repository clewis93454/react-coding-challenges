# Chatter Coding Challenge 🤖 &nbsp; ![hard](https://img.shields.io/badge/-Hard-red) ![time](https://img.shields.io/badge/%E2%8F%B0-60m-blue)
&nbsp;
# Requirements 📖
Most of the work needs to be done in the `Messages` components.
`chatter/src/components/Messages/components/Messages.js`

- Display messages (both sent and received)
- Implement hooks such as `useEffect` and `useCallback` to handle events (sending/receiving messages)
- Use **sockets** to:
  - Send the user's message to Botty
  - Show a typing message when Botty is typing
  - Handle incoming Botty messages and display them
  - Documentation: https://socket.io/
- Implement audio cues for sending/receiving messages
- Scroll to the bottom of the messages list when sending/receiving a message

&nbsp;
# What's Already Been Done 🏁
- Socket setup/configuration with the [Botty server](https://github.com/alexgurr/botty) ([botty.alexgurr.com](https://botty.alexgurr.com))
- All UX and UI, including for messages
- All components, including a message and typing message component
- A context for setting the latest message, which will change the preview in the left user list
- Hooks for playing send/receive sounds

&nbsp;
# Botty Socket Events
See the [Botty server](https://github.com/alexgurr/botty) documentation for more information.
- `bot-typing`: Emitted by Botty when they are typing in response to a user message.
- `bot-message`: Emitted by Botty with a message payload in response to a user message.
- `user-message`: Emitted by you/the client with a messsage payload

&nbsp;
# Message Classes
We've provided `Message` components and classes. Here's some information about the classes.
- `.message--last`: The last message in a group
- `.message--typing`: The message the user sees when the recipient is typing
- `.message--me`: Denotes a user message

&nbsp;
# Think about 💡
- References to functions and current hook state
- How to interact with socket.io, events and payloads
- How React contexts work

&nbsp;
# Screenshots 🌄
&nbsp;
![screenshot-desktop](https://puu.sh/Hp0C2/cb14e843de.png)
<img alt="screenshot-mobile" width=400 src="https://puu.sh/HoYEw/9b760f91f7.png" />
