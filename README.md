# Imaginize

Imaginize is an advanced image transformation service that allows users to perform various image editing tasks such as image restoration, generative fill, object removal, object recolor, and background removal. The service operates on a freemium model, providing basic functionalities for free and offering additional credits for extended usage.

## Features

- **Image Restore**: Bring old or damaged photos back to life with advanced restoration techniques.
- **Generative Fill**: Fill in missing parts of an image with AI-generated content.
- **Object Remove**: Effortlessly remove unwanted objects from your images.
- **Object Recolor**: Change the color of specific objects within your images.
- **Background Remove**: Remove or replace the background of your images.

## Technology Stack

- **Next.js**: A React framework used for building the user interface of Imaginize.
- **Stripe**: A payment processing platform used to handle purchases of additional credits.
- **MongoDB**: A NoSQL database used to store user data, image metadata, and transaction records.
- **Cloudinary SDK**: A cloud-based image and video management service used for image transformation operations.
- **Clerk**: A user management platform used for authentication and user management.

## Installation

To set up Imaginize locally, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/imaginize.git
    cd imaginize
    ```

2. **Install dependencies**:
    ```bash
    npm install
    ```

3. **Set up environment variables**:
    Create a `.env.local` file in the root directory and add the following variables:
    ```
    #NEXT
    NEXT_PUBLIC_SERVER_URL=

    #MONGODB
    MONGODB_URL=

    #CLERK
    NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
    CLERK_SECRET_KEY=
    WEBHOOK_SECRET=

    NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
    NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
    NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
    NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

    #CLOUDINARY
    NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=
    CLOUDINARY_API_KEY=
    CLOUDINARY_API_SECRET=

    #STRIPE
    STRIPE_SECRET_KEY=
    STRIPE_WEBHOOK_SECRET=
    NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=
    ```

4. **Run the development server**:
    ```bash
    npm run dev
    ```

    Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Usage

1. **Sign Up / Log In**: Create an account or log in to your existing account.
2. **Upload Image**: Upload the image you want to transform.
3. **Select Feature**: Choose the desired transformation feature (e.g., Image Restore, Generative Fill, etc.).
4. **Apply Transformation**: Apply the transformation and review the result.
5. **Download**: Download the transformed image to your device.
6. **Purchase Credits**: If you need more transformations, purchase additional credits via Stripe.

## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
