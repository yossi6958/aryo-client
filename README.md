# Aryo

"Learn, Teach, and Grow with Aryo – Your Gateway to Knowledge and Opportunity."

## About Aryo

Aryo is an all-in-one platform for learners and instructors. Explore a diverse range of courses to enhance your skills, or create and sell your own courses to share your expertise with a global audience. Whether you're learning or teaching, Aryo makes knowledge accessible and empowering for everyone.

## For Developers

### Extensions

Beside the common extensions for VsCode you should also make sure you have:

1. ES7+ React/Redux/React-Native snippets by dsznajder.
2. Prettier by Prettier.
3. Tailwind CSS IntelliSense by Tailwind Labs.
4. Tailwind Documentation by alfredbirk.

### Chrome Tools

You should have:

1. Pesticide for Chrome
2. Redux DevTools

## Frontend

I have created the client using:
`npx create-next-app@latest`

### Client Dependencies

`cd client`

We have added `--legacy-peer-deps` flag to be compatible with Next and React Versions

`npm i lucide-react uuid dotenv date-fns framer-motion react-hook-form zod @hookform/resolvers @hello-pangea/dnd --legacy-peer-deps`

#### Tailwind

`npm i tailwindcss-animate --legacy-peer-deps`

#### Shadcn

In shadcn always choose --legacy-peer-deps option

`npx shadcn@latest init -d`

`npx shadcn@latest add accordion avatar button card dialog form input label navigation-menu popover progress select separator sheet sidebar skeleton switch table tabs textarea toggle tooltip`

#### Redux

`npm i react-redux @reduxjs/toolkit --legacy-peer-deps`

#### Clerk

`npm i @clerk/clerk-js @clerk/nextjs @clerk/themes next themes --legacy-peer-deps`

#### Stripe

`npm i @stripe/react-stripe-js @stripe/stripe-js --legacy-peer-deps`

### Client Dev Dependencies

`cd client`

`npm i -D @types/node @types/uuid prettier-plugin-tailwindcss --legacy-peer-deps`

### Env Variables

you should create `.env{.local/.development/.deployment}` with Variables same as `.env.example`

## Backend

I have created the server using:
`cd server`
`npm init -y`

### Server Dependencies

`npm i @aws-sdk/client-dynamodb aws-sdk body-parser express cors dotenv helmet morgan dynamoose uuid pluralize`

#### Stripe for Server

`npm i stripe`

### Server Dev Dependencies

`npm i -D rimraf concurrently nodemon ts-node typescript @types/cors @types/express @types/morgan @types/node @types/uuid @types/pluralize`

`npx tsc --init`

## AWS

### DynamoDB

`java -Djava.library.path={LOCAL_PATH}\dynamodb-local\DynamoDBLocal_lib -jar {LOCAL_PATH}\dynamodb-local\DynamoDBLocal.jar -sharedDb -dbPath {LOCAL_PATH}\dynamodb-local\run`

`aws dynamodb list-tables --endpoint-url http://localhost:8000`

#### seeding mock data

`npm run seed`
