![StoreIt Cover Image](public/cover-image.png)

# StoreIt

StoreIt is a digital storage application, similar to Google Drive, allowing users to store and manage their files online. Built with **Next.js 15**, **Appwrite**, **shadcn/ui** and **TailwindCSS**, StoreIt provides a seamless and user-friendly interface for secure file storage.

## Features

- **File Upload:** Upload and store files securely.
- **Storage Limit:** Maximum total storage of **2GB** per user.
- **File Size Limit:** Maximum file size of **20MB** for individual uploads.
- **User Authentication:** Secure login and registration using Appwrite.
- **Responsive Design:** Mobile-friendly interface powered by TailwindCSS.

## Tech Stack

- **Frontend:** [Next.js 15](https://nextjs.org/)
- **Backend:** [Appwrite](https://appwrite.io/)
- **Styling:** [TailwindCSS](https://tailwindcss.com/), [shadcn/ui](https://ui.shadcn.com/)

## Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v16 or higher)
- [NPM](https://www.npmjs.com/) or [Yarn](https://yarnpkg.com/)
- An Appwrite instance (local or cloud)

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/storeit.git
   cd storeit
   ```

2. **Install dependencies:**

   ```bash
   npm install
   # or
   yarn install
   ```

3. **Configure Appwrite:**

   - Set up an Appwrite project.
   - Create a database for storing file metadata.
   - Update the `appwriteConfig` in the `lib` folder with your Appwrite project's details:

     ```javascript
     const appwriteConfig = {
       endpointUrl: "https://your-appwrite-endpoint.io/v1",
       projectId: "your-project-id",
     };
     export default appwriteConfig;
     ```

4. **Start the development server:**

   ```bash
   npm run dev
   # or
   yarn dev
   ```

5. **Access the application:**

   Open your browser and navigate to `http://localhost:3000`.

## Usage

1. **Sign In/Sign Up:** Create an account or log in using your credentials.
2. **Upload Files:** Navigate to the upload section to upload files (max 20MB per file).
3. **Manage Files:** View and delete uploaded files.


## Environment Variables

Create a `.env.local` file in the root of your project and add the following variables:

```plaintext
NEXT_PUBLIC_APPWRITE_ENDPOINT="https://cloud.appwrite.io/v1"
NEXT_PUBLIC_APPWRITE_PROJECT="67386f0400017f2f9216"
NEXT_PUBLIC_APPWRITE_DATABASE="67386fd3002132a9dbc4"
NEXT_PUBLIC_APPWRITE_USERS_COLLECTION="6738700b003d47fe2e64"
NEXT_PUBLIC_APPWRITE_FILES_COLLECTION="673870ff002d20487549"
NEXT_PUBLIC_APPWRITE_BUCKET="673873c3002e15fa1892"
NEXT_APPWRITE_KEY="standard_e27481ab6711d5385183f53a78d84d3509e603fd05b543954f25b6b29edebd7630da125f879bc84cef4b30882e69b3874c46c85e81fdb7a860147023a2adbdcdaae898b0739ab74fcfafb3806cea89bb8c733238a736d05277ee9ce8fb1045d6a672dd583292504ed5ef760d2cebefde67f7ea2be10b384384892c8c98a0c8a8"
```

## Limitations

- **Storage:** Each user is limited to 2GB of total file storage.
- **File Size:** Individual files cannot exceed 20MB.


## Acknowledgements

- [Next.js](https://nextjs.org/)
- [Appwrite](https://appwrite.io/)
- [TailwindCSS](https://tailwindcss.com/)
- [Shadcn/ui](https://ui.shadcn.com/)

---

Feel free to reach out if you have any questions or issues with StoreIt!
