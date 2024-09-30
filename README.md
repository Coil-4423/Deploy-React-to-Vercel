To deploy your React project (with Next.js) to Vercel using your GitHub repository, follow these steps:

### Step 1: Push Your Code to GitHub

Make sure your code is already committed and pushed to your GitHub repository.

1. **Initialize Git** if you haven’t already in your project folder:
   ```bash
   git init
   ```

2. **Add the remote GitHub repository** if you haven’t already:
   ```bash
   git remote add origin https://github.com/yourusername/your-repository.git
   ```

3. **Add your files, commit, and push**:
   ```bash
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```

Replace `main` with `master` if that's the branch name you're using.

### Step 2: Sign Up/Login to Vercel

1. **Go to Vercel**: Visit [vercel.com](https://vercel.com/) and sign up (if you haven't) or log in.
   
2. **Connect GitHub to Vercel**: 
   - After logging in, Vercel will ask you to link your GitHub account. Click on the **GitHub** option.
   - Authorize Vercel to access your repositories.
   
### Step 3: Create a New Project in Vercel

1. **New Project**: After connecting GitHub, you'll be directed to the Vercel dashboard.
   - Click on **New Project**.
   
2. **Import Repository**: 
   - Choose the repository you want to deploy from GitHub.

### Step 4: Configure and Deploy

1. **Project Configuration**: 
   - Vercel should automatically detect your project type (since you're using Next.js) and configure it for you. If needed, you can customize the build settings (usually not necessary for Next.js).
   
2. **Environment Variables (Optional)**: 
   - If your project uses any environment variables (like API keys or API URLs), you can add them under the **Environment Variables** section.

3. **Deploy**: 
   - Click the **Deploy** button. Vercel will now build and deploy your project.

### Step 5: View Your Deployed Project

Once the deployment is finished, Vercel will provide you with a URL (something like `your-app.vercel.app`). This is your live site URL, and you can visit it to see your deployed React app.

### Step 6: Set Up Automatic Deployments (Optional)

Vercel will automatically set up continuous deployment for your project. This means every time you push new code to your GitHub repository (on the `main` branch or whichever branch you linked), Vercel will automatically rebuild and redeploy your site.

### Optional Configuration

1. **Custom Domain**: If you have a custom domain, you can add it by going to the Vercel dashboard under the project's settings, then linking your custom domain.

2. **Environment Variables**: 
   - Go to the project’s settings on Vercel, and add any necessary environment variables if needed (like `NEXT_PUBLIC_API_URL` for API endpoints).

### Step-by-Step Summary

1. Push your React/Next.js code to GitHub.
2. Sign in to [Vercel](https://vercel.com/).
3. Connect your GitHub account to Vercel.
4. Select the repository you want to deploy.
5. Deploy the project and get your live site URL.
6. Push code to GitHub for automatic redeployment.
