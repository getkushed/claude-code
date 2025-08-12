---
allowed-tools: Bash(gh workflow run:*), Bash(gh workflow list:*), Bash(gh api:*)
description: Generate mobile-friendly GitHub Actions workflows with smart naming
---

## Mobile Workflow Generator

Generate GitHub Actions workflows optimized for mobile users with intelligent naming conventions and templates.

### 📱 Mobile-First Commands

**Quick Generation:**
- `/mobile-workflow name:my-app` - Generate mobile-optimized CI workflow
- `/claude-generate name:lint-check` - Create Claude-powered analysis workflow  
- `/auto-workflow name:deploy-app` - Build automated deployment workflow

### 🎯 Smart Naming System

The system automatically applies intelligent prefixes:
- **mobile-*** - CI, testing, and mobile-specific workflows
- **claude-*** - AI-powered code analysis and review workflows
- **auto-*** - Automated deployment and maintenance workflows

### 📋 Available Templates

1. **ci-basic** - Mobile-optimized CI/CD pipeline
   - Fast execution (< 10 minutes)
   - Mobile-friendly status notifications
   - Essential build and test steps

2. **deploy-auto** - Automated deployment workflows  
   - Environment selection (dev/staging/prod)
   - Mobile-friendly deployment confirmations
   - Rollback capabilities

3. **test-mobile** - Mobile-specific testing
   - Quick test execution
   - Mobile-optimized test reporting
   - Cross-platform compatibility checks

4. **lint-claude** - Claude-powered code analysis
   - Intelligent code review
   - Mobile-friendly feedback format
   - Integration with Claude Code API

5. **security-scan** - Security vulnerability scanning
   - Mobile-friendly security reports
   - Scheduled and on-demand scanning
   - Clear vulnerability summaries

### 🚀 Usage Examples

**Basic CI Workflow:**
```
/mobile-workflow name:my-react-app template:ci-basic
```

**Claude-Powered Linting:**
```  
/claude-generate name:code-review template:lint-claude
```

**Auto-Deployment:**
```
/auto-workflow name:prod-deploy template:deploy-auto
```

### 📱 Mobile Optimization Features

- **Fast Execution:** All workflows optimized for < 15 minute completion
- **Mobile Notifications:** Clear, concise status updates for mobile devices
- **Simple UI:** Easy-to-read workflow names and descriptions
- **Touch-Friendly:** Commands designed for mobile input
- **Quick Access:** Direct links to workflow runs and settings

### 🔧 Manual Generation

For advanced options, use the manual workflow dispatch:
1. Go to repository Actions tab
2. Select "Mobile Workflow Generator"
3. Click "Run workflow" 
4. Configure options via mobile-friendly form

### 📞 Getting Help

- Comment `/mobile-help` for detailed assistance
- Tag `@claude` with specific questions
- Check existing workflows for examples

### 🔒 Security Features

- **Input Validation:** All inputs sanitized and validated
- **Secure Defaults:** Minimal required permissions
- **Error Handling:** Comprehensive error recovery
- **Audit Trail:** Complete generation history

*This command integrates with the Mobile Workflow Generator action for seamless workflow creation.*