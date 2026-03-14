# Klondike Solitaire

A lightweight HTML5 solitaire game optimized for old tablets. Deploys to GitHub Pages automatically.

## Features
- Single HTML file (~15 KB) - extremely fast loading
- Touch-friendly for tablets
- No dependencies or frameworks
- Works offline once loaded

## How to Deploy to GitHub Pages

### 1. Create a GitHub Repository

```bash
# Navigate to the project folder
cd C:\Users\jules\Documents\7cardsolitair

# Create the repository on GitHub first, then clone it
git init
```

### 2. Configure GitHub Pages

Once your repository is created on GitHub:

1. Go to your repository on GitHub
2. Click **Settings** → **Pages**
3. Under **Build and deployment**, select:
   - **Branch**: `main` (or `master`)
   - **Folder**: `/ (root)`
4. Click **Save**

### 3. Push the Code

```bash
git add .
git commit -m "Initial solitaire game"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

### 4. Access Your Game

GitHub Pages will be available at:
```
https://YOUR_USERNAME.github.io/YOUR_REPO/
```

## For Your Grandpa

Simply:
1. Create a GitHub repository (e.g., `7card-solitaire`)
2. Follow the setup above
3. Share the GitHub Pages URL with your grandpa
4. He can play directly in his tablet browser - no app store or account needed!

## How to Play

- **Stock** (left): Click to draw cards
- **Waste** (next to stock): Discard pile for drawn cards
- **Foundations** (top right): Build up by suit from Ace to King
- **Tableau** (bottom): Build down alternating colors
  - Kings go in empty spots
  - Click stock to cycle cards

## Customizing

To change the card back design, edit CSS lines 41-47:
```css
.card.face-down {
    background: linear-gradient(135deg, #1a237e 0%, #0d1442 100%);
    background-image: repeating-linear-gradient(...);
    border: 2px solid #283593;
}
```

## License

Create your own license or use MIT license.
