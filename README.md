## 🚀 Quick Start

### 1. Installation

```bash
# Clone the repository
git clone https://github.com/your-username/github-hero.git
cd github-hero

# Install dependencies
pip3 install -r requirements.txt
```

### 2. Configuration

```bash
# Copy the example configuration
cp config.example.json config.json

# Edit config.json with your GitHub credentials
nano config.json
```

**Required GitHub Token Permissions:**
- `repo` (Full control of private repositories)
- `public_repo` (Access public repositories)

### 3. Usage

```bash
python3 github_hero.py
```

## 📋 Configuration

Create a `config.json` file with your GitHub credentials:

```json
{
  "github_username": "your-github-username",
  "github_email": "your-email@example.com",
  "github_token": "your-github-personal-access-token",
  "repos_dir": "repos"
}
```

### Getting GitHub Personal Access Token

1. Go to GitHub Settings → Developer settings → Personal access tokens
2. Click "Generate new token (classic)"
3. Select scopes: `repo`, `public_repo`
4. Copy the generated token

## 🎯 Usage Modes

### 1. Historical Commits
Creates backdated commits for 2023-2025 to show long-term activity.

```bash
python3 github_hero.py
# Select option 1
```

### 2. PR & Issues
Generates Pull Requests and Issues with realistic content.

```bash
python3 github_hero.py
# Select option 2
```

### 3. Daily Change
Makes random daily commits to keep your profile active.

```bash
python3 github_hero.py
# Select option 3
```

### 4. Mass Activity
Creates maximum activity with lots of PRs and Issues.

```bash
python3 github_hero.py
# Select option 4
```

### 5. All Modes
Runs all modes sequentially for complete activity generation.

```bash
python3 github_hero.py
# Select option 5
```

## 📊 What Gets Created

### Historical Commits
- Backdated commits from 2023-2025
- Realistic commit messages
- Code changes and documentation updates
- 2 commits per month per repository

### Pull Requests
- Feature implementations
- Bug fixes
- Performance improvements
- Security enhancements
- All PRs are automatically merged

### Issues
- Bug reports
- Feature requests
- Improvement suggestions
- All Issues are automatically closed

### Daily Changes
- Random code modifications
- Documentation updates
- Small feature additions
- Bug fixes

## 🛠️ Technical Details

### Supported File Types
- Python (`.py`)
- JavaScript (`.js`, `.ts`)
- JSON (`.json`)
- Markdown (`.md`)

### Repository Requirements
- Must be owned by your GitHub account
- Must have at least one file
- Supports both `main` and `master` branches

### API Usage
- Uses GitHub REST API v3
- Respects GitHub rate limits
- Includes proper error handling

## 🔒 Security & Privacy

- **No Data Collection** - All activity is local to your repositories
- **Secure Configuration** - Credentials stored locally in config.json
- **Rate Limiting** - Respects GitHub API limits
- **Error Handling** - Graceful failure with detailed error messages



## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⚠️ Disclaimer

This tool is for educational and personal use. Please use responsibly and in accordance with GitHub's Terms of Service. The generated activity should represent realistic development work and not be used to misrepresent your actual coding abilities.

## 🆘 Support

If you encounter any issues:

1. Check that your GitHub token has the correct permissions
2. Ensure your repositories exist and are accessible
3. Verify your internet connection
4. Check the error messages for specific issues
