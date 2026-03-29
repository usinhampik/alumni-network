# Contributing to the Alumni Network

Welcome to the Alumni Network! This document will guide you through the steps to add your profile to the network.

## Step-by-Step Instructions

1. **Fork the Repository**  
   Click on the 'Fork' button at the top right of this page to create a copy of this repository under your own GitHub account.

2. **Clone Your Fork**  
   Clone your forked repository to your local machine using the following command:
   ```bash
   git clone https://github.com/YOUR-USERNAME/alumni-network.git
   ```

3. **Create a New Branch**  
   Navigate to the cloned directory and create a new branch for your profile:
   ```bash
   cd alumni-network
   git checkout -b add-my-profile
   ```

4. **Add Your Profile**  
   Add a new file named `YOUR-NAME.md` in the appropriate directory (e.g., `profiles/`).
   The profile file should include your name, graduation year, degree, and a brief bio.

5. **Commit Your Changes**  
   Stage the new file and commit your changes with a relevant message:
   ```bash
   git add profiles/YOUR-NAME.md
   git commit -m "Add profile for YOUR NAME"
   ```

6. **Push to Your Fork**  
   Push your changes to your forked GitHub repository:
   ```bash
   git push origin add-my-profile
   ```

7. **Create a Pull Request**  
   Go to your forked repository on GitHub and click on 'New Pull Request'. Choose the branch you just pushed and create the pull request to merge into the `main` branch of the original repository.

8. **Wait for Review**  
   Once your pull request is submitted, the maintainers will review your profile. You may need to respond to comments or make further changes.

9. **Celebrate!**  
   After your pull request is merged, congratulate yourself on joining the Alumni Network!