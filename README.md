# Nerdy Chat 🤓

Nerdy Chat is a chat application that allows users to chat with each other in real time. Users can create chat rooms and invite other users to join them! 🚀

By the moment it's a Discord clone, but in the future, it will be a chat application with its own identity, with its own features and functionalities. The objective audience is the nerdy community, like academics, developers, gamers, mathematicians, etc., and even more, the people who want to learn about these topics, so you can create a chat room with a school-like environment, made for teachers, students, and if applies, parents! 🤓

## How was it built? 🤔 
This project was built using Next.js, TypeScript, Clerk, PlanetScale, Prisma, Socket.io, TailwindCSS, LiveKit, and deployed using Railway. 🚀

## How to run it locally? 🚀
First, clone our repository:
```bash
git clone https://github.com/MathItYT/nerdy.chat.git
```

Then, install the dependencies:
```bash
npm install
```

Create a `.env` file with the following content:
```bash
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=<CLERK_PUBLISHABLE_KEY>
CLERK_SECRET_KEY=<CLERK_SECRET_KEY>

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

# PlanetScale
DATABASE_URL=<DATABASE_URL>

UPLOADTHING_SECRET=<UPLOADTHING_SECRET>
UPLOADTHING_APP_ID=<UPLOADTHING_APP_ID>

LIVEKIT_API_KEY=<LIVEKIT_API_KEY>
LIVEKIT_API_SECRET=<LIVEKIT_API_SECRET>
NEXT_PUBLIC_LIVEKIT_URL=<NEXT_PUBLIC_LIVEKIT_URL>
```

Update the Prisma Client:
```bash
npx prisma generate
npx prisma db push
```

Finally, run the development server:
```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result. 🎉

## Known bugs 🐛
- Cannot sign-out on mobile devices.
- Cannot manage account on mobile devices.
- There's no error when the user sets an username without the correct format on mobile devices. It instead shows a blank page.

## Contributing 🤝
If you know any bug that isn't listed above, fix one of the listed bugs, or you want to add a new feature, feel free to open an issue or a pull request! 🚀
