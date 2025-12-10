# MkDocs Template with Multiple Deployment Options

A comprehensive MkDocs documentation template with multiple deployment strategies, custom enhancements, and production-ready configurations.

## 🚀 Features

### **Documentation**
- ✅ **MkDocs** with ReadTheDocs theme
- ✅ **Custom CSS** with enhanced styling
- ✅ **Copy-to-clipboard** functionality for code blocks
- ✅ **Syntax highlighting** for multiple programming languages
- ✅ **Responsive design** optimized for all devices
- ✅ **Comprehensive formatting guide** with examples

### **Deployment Options**
- ✅ **GitHub Pages** (Official method + gh-deploy)
- ✅ **GitLab Pages** (Cross-platform integration)
- ✅ **Production Server** (SSH/SCP deployment)
- ✅ **Local development** with live reload

### **Developer Experience**
- ✅ **Requirements management** with pip
- ✅ **GitHub Actions** workflows (templates)
- ✅ **Comprehensive setup guides**
- ✅ **Copy button** for code blocks
- ✅ **Professional footer** with copyright

## 📁 Project Structure

```
mkdocs-template/
├── docs/                           # MkDocs source directory
│   ├── docs/                       # Documentation content
│   │   ├── index.md               # Home page
│   │   ├── about.md               # About the theme
│   │   ├── format.md              # Markdown formatting guide
│   │   ├── css/                   # Custom stylesheets
│   │   │   └── custom.css         # Enhanced styling + copy buttons
│   │   ├── js/                    # Custom JavaScript
│   │   │   └── copy-code.js       # Copy-to-clipboard functionality
│   │   └── img/                   # Images and assets
│   │       └── favicon.ico
│   ├── .github/                    # GitHub Actions workflows
│   │   ├── workflows/             # Deployment templates
│   │   │   ├── *.yml.template     # Inactive workflow templates
│   │   │   └── [active].yml       # Active workflow
│   │   ├── GITHUB_PAGES_SETUP.md  # GitHub Pages setup guide
│   │   ├── GITLAB_PAGES_SETUP.md  # GitLab Pages setup guide
│   │   └── PRODUCTION_DEPLOY_SETUP.md # Production deployment guide
│   ├── mkdocs.yml                 # MkDocs configuration
│   ├── requirements.txt           # Python dependencies
│   └── site/                      # Generated static files (build output)
└── README.md                      # This file
```

## 🛠️ Quick Start

### **Prerequisites**
- Python 3.x
- pip package manager
- Git

### **Local Development**

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd mkdocs-template/docs
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Start development server**
   ```bash
   mkdocs serve
   ```

4. **Access your site**
   - Open http://127.0.0.1:8000 in your browser
   - Changes auto-reload for instant preview

### **Build for Production**
```bash
mkdocs build
```
Generated files will be in the `site/` directory.

## 🌐 Deployment Options

This template includes multiple deployment strategies. Choose the one that fits your needs:

### **1. GitHub Pages** 
**Best for**: Open source projects, simple hosting

**Templates available:**
- `github-pages-deploy.yml.template` - Official GitHub Pages method
- `github-pages-build.yml.template` - Traditional gh-deploy method

**Setup**: See `.github/GITHUB_PAGES_SETUP.md`

### **2. GitLab Pages**
**Best for**: GitLab users, cross-platform development

**Templates available:**
- `gitlab-pages-build.yml.template` - Build and update gl-pages branch
- `gitlab-pages-deploy.yml.template` - Deploy to GitLab Pages

**Setup**: See `.github/GITLAB_PAGES_SETUP.md`

### **3. Production Server**
**Best for**: Self-hosted solutions, custom domains, enterprise

**Templates available:**
- `simple-production-deploy.yml.template` - Minimal SSH/SCP deployment
- `extensive-production-deploy.yml.template` - Full-featured production deployment

**Setup**: See `.github/PRODUCTION_DEPLOY_SETUP.md`

## 🎨 Customization

### **Site Configuration**
Edit `mkdocs.yml`:
```yaml
site_name: Your Project Name
site_url: https://yoursite.com
copyright: Copyright &copy; 2025 Your Name

nav:
  - Home: index.md
  - Your Page: your-page.md
```

### **Styling**
- **Custom CSS**: Edit `docs/css/custom.css`
- **Theme colors**: Modify CSS variables
- **Copy button styling**: Customize `.copy-button` class

### **Content**
- **Add pages**: Create `.md` files in `docs/`
- **Update navigation**: Edit `nav` section in `mkdocs.yml`
- **Add images**: Place in `docs/img/`

### **Code Highlighting**
Supported languages (configurable in `mkdocs.yml`):
- Python, JavaScript, Rust, C/C++, Java
- Bash/Shell, YAML, JSON, Markdown

## 🔧 Advanced Features

### **Copy-to-Clipboard**
- **Hover activation**: Copy buttons appear on code block hover
- **One-click copying**: Instant clipboard access
- **Visual feedback**: "Copied!" confirmation
- **Cross-browser support**: Works in modern and legacy browsers

### **Professional Footer**
- **Copyright notice**: Customizable copyright information
- **Responsive design**: Looks great on all devices
- **Clean styling**: Professional appearance

### **Enhanced Code Blocks**
- **Syntax highlighting**: Multiple language support
- **Clean presentation**: Optimized for readability
- **Copy functionality**: Built-in copy buttons

## 📚 Documentation Pages

### **Included Pages:**
- **`index.md`** - Welcome page with project overview
- **`about.md`** - Detailed theme and setup information
- **`format.md`** - Comprehensive Markdown formatting guide

### **Formatting Guide Features:**
- Complete Markdown syntax reference
- ReadTheDocs theme-specific examples
- Code highlighting demonstrations
- Best practices and common mistakes
- Live examples with side-by-side syntax/output

## 🚀 Deployment Activation

### **Activate a Deployment Method:**

1. **Choose your deployment strategy**
2. **Rename the template file**:
   ```bash
   # Example: Activate GitHub Pages
   cd .github/workflows
   ren github-pages-deploy.yml.template github-pages-deploy.yml
   ```
3. **Follow the setup guide** for your chosen method
4. **Commit and push** to trigger deployment

### **Multiple Environments:**
You can activate multiple workflows for different environments:
- `github-pages-deploy.yml` - For GitHub Pages
- `production-deploy.yml` - For production server
- Keep others as `.template` for future use

## 🛡️ Security Features

### **GitHub Actions Security:**
- **Minimal permissions**: Workflows use least-privilege access
- **Secret management**: Sensitive data stored in repository secrets
- **SSH key cleanup**: Automatic removal of temporary keys
- **Host verification**: SSH host key validation

### **Deployment Safety:**
- **Build verification**: Ensures successful build before deployment
- **Backup creation**: Optional pre-deployment backups
- **Rollback capability**: Easy reversion to previous versions
- **Error handling**: Comprehensive failure detection and reporting

## 📖 Setup Guides

Detailed setup instructions are available for each deployment method:

- **[GitHub Pages Setup](.github/GITHUB_PAGES_SETUP.md)** - Complete GitHub Pages configuration
- **[GitLab Pages Setup](.github/GITLAB_PAGES_SETUP.md)** - Cross-platform GitLab deployment
- **[Production Deployment](.github/PRODUCTION_DEPLOY_SETUP.md)** - Self-hosted server setup

## 🤝 Contributing

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/amazing-feature`
3. **Make your changes**
4. **Test locally**: `mkdocs serve`
5. **Commit changes**: `git commit -m 'Add amazing feature'`
6. **Push to branch**: `git push origin feature/amazing-feature`
7. **Open a Pull Request**

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🏗️ Built With

- **[MkDocs](https://www.mkdocs.org/)** - Static site generator
- **[ReadTheDocs Theme](https://www.mkdocs.org/user-guide/choosing-your-theme/)** - Clean documentation theme
- **[GitHub Actions](https://github.com/features/actions)** - CI/CD automation
- **[Python](https://www.python.org/)** - Build environment

## 📞 Support

- **Documentation Issues**: Open an issue in this repository
- **Deployment Help**: Check the setup guides in `.github/`
- **Feature Requests**: Submit via GitHub Issues
- **Questions**: Use GitHub Discussions

## 🔄 Version History

- **v1.0.0** - Initial release with multiple deployment options
<!-- - **v1.1.0** - Added copy-to-clipboard functionality
- **v1.2.0** - Enhanced GitHub Actions workflows
- **v1.3.0** - Added GitLab Pages support -->

## 🌟 Acknowledgments

- **MkDocs Team** - For the excellent static site generator
- **ReadTheDocs** - For the clean, professional theme
- **GitHub Actions Community** - For deployment workflow inspiration
- **Contributors** - For improvements and bug fixes

---

**Ready to get started?** Choose your deployment method and follow the corresponding setup guide!

**Questions?** Check out the documentation pages or open an issue.
