# Mobile-Friendly Workflow Generator

A GitHub Actions workflow system optimized for mobile users, featuring smart naming conventions, template-based generation, and Claude integration.

## 🚀 Quick Start

### For Mobile Users

1. **Comment Commands** (easiest for mobile):
   ```
   /mobile-workflow name:my-app
   /claude-generate name:lint-check  
   /auto-workflow name:deploy-prod
   ```

2. **Manual Dispatch** (via GitHub mobile app):
   - Navigate to Actions → Mobile Workflow Generator
   - Tap "Run workflow" 
   - Select template and enter name
   - Tap "Run workflow"

## 🎯 Smart Naming System

The system automatically applies intelligent prefixes based on workflow type:

| Prefix | Use Case | Examples |
|--------|----------|----------|
| `mobile-` | CI, testing, mobile-specific workflows | `mobile-react-ci`, `mobile-test-suite` |
| `claude-` | AI-powered analysis and review | `claude-code-review`, `claude-lint-check` |
| `auto-` | Automated deployment and maintenance | `auto-deploy-prod`, `auto-update-deps` |

### Naming Rules
- Invalid characters automatically converted to hyphens
- Maximum 50 characters (GitHub limit)
- Duplicate prefixes automatically detected and removed
- Case-insensitive processing

## 📋 Workflow Templates

### 1. CI Basic (`ci-basic`)
**Best for:** Basic continuous integration
```yaml
# Features:
- Fast execution (< 10 minutes)
- Mobile-friendly notifications
- Essential build and test steps
- Cross-platform support
```

### 2. Deploy Auto (`deploy-auto`)  
**Best for:** Automated deployments
```yaml
# Features:
- Environment selection (dev/staging/prod)
- Mobile deployment confirmations
- Rollback capabilities
- Security validations
```

### 3. Test Mobile (`test-mobile`)
**Best for:** Mobile-specific testing
```yaml
# Features:
- Quick test execution (< 8 minutes)
- Mobile-optimized reporting
- Cross-platform compatibility
- Parallel test execution
```

### 4. Lint Claude (`lint-claude`)
**Best for:** AI-powered code analysis
```yaml
# Features:
- Claude Code integration
- Intelligent code review
- Mobile-friendly feedback
- Automated suggestions
```

### 5. Security Scan (`security-scan`)
**Best for:** Security analysis
```yaml
# Features:
- Vulnerability scanning
- Mobile security reports
- Scheduled and on-demand
- Compliance checking
```

## 📱 Mobile Optimization Features

### Interface Optimizations
- **Touch-Friendly Commands:** Simple slash commands for mobile typing
- **Quick Templates:** Pre-configured workflows for common use cases  
- **Smart Defaults:** Sensible configuration with minimal input required
- **Clear Feedback:** Mobile-optimized success/failure messages

### Performance Optimizations  
- **Fast Execution:** All templates optimized for < 15 minute completion
- **Efficient Resource Usage:** Minimal compute requirements
- **Quick Feedback:** Immediate status updates and notifications
- **Mobile App Integration:** GitHub mobile app compatible

### Notification System
- **Clear Messages:** Concise, actionable status updates
- **Mobile Format:** Optimized for small screen reading
- **Quick Actions:** Direct links to workflow runs and settings
- **Error Recovery:** Helpful troubleshooting for mobile users

## 🔧 Advanced Usage

### Custom Template Parameters
```bash
# Custom workflow with specific parameters
/mobile-workflow name:custom-app template:ci-basic env:production timeout:20
```

### Manual Configuration
Use the workflow_dispatch interface for advanced options:
- Custom environment variables
- Specific trigger conditions
- Advanced notification settings
- Custom timeout values

## 🔒 Security Features

### Input Validation
- **Sanitization:** All inputs cleaned and validated
- **Length Limits:** Prevents excessively long names
- **Character Filtering:** Only safe characters allowed
- **Template Validation:** Generated workflows validated before saving

### Permission Management
- **Minimal Access:** Only required permissions granted
- **Secure Defaults:** Conservative security settings
- **Token Management:** Secure handling of authentication tokens
- **Audit Trail:** Complete generation history logged

### Error Handling
- **Graceful Failures:** Clear error messages for mobile users
- **Recovery Options:** Automated retry mechanisms
- **Fallback Templates:** Backup options if primary template fails
- **Debug Information:** Helpful troubleshooting data

## 🎛️ Configuration

### Environment Variables
```yaml
# Available in workflow environment
MOBILE_MODE: "true"
WORKFLOW_PREFIX: "mobile-|claude-|auto-"  
NOTIFICATION_MODE: "mobile"
TIMESTAMP: "YYYYMMDD-HHMMSS"
```

### Secrets Required
- `GITHUB_TOKEN` - Repository access (automatically provided)
- `ANTHROPIC_API_KEY` - Claude integration (for claude-* workflows)

## 📞 Support & Help

### Getting Help
- **Quick Help:** Comment `/mobile-help` for immediate assistance
- **Claude Integration:** Tag `@claude` with specific questions
- **Documentation:** Check existing workflows for examples
- **Community:** Search issues for similar problems

### Common Issues

**Issue:** Workflow name too long
**Solution:** Use shorter, descriptive names (< 50 characters)

**Issue:** Template not found  
**Solution:** Use one of the five available templates: `ci-basic`, `deploy-auto`, `test-mobile`, `lint-claude`, `security-scan`

**Issue:** Command not recognized
**Solution:** Ensure proper format: `/command-type name:workflow-name`

## 🚦 Status & Monitoring

### Workflow Status
- **Success:** Green checkmark, mobile-friendly success message
- **Failure:** Red X, detailed error information with recovery steps  
- **In Progress:** Yellow circle, real-time progress updates
- **Cancelled:** Gray circle, cancellation reason provided

### Mobile App Integration
- GitHub mobile app shows workflow status in notifications
- Direct links to workflow runs for easy access
- Push notifications for workflow completion
- Quick actions available from notification interface

## 🔄 Updates & Maintenance

The Mobile Workflow Generator is designed to be self-maintaining:
- **Template Updates:** Automatically pulls latest template versions
- **Security Patches:** Regular security updates applied automatically  
- **Performance Optimization:** Continuous monitoring and improvement
- **Mobile Compatibility:** Regular testing with GitHub mobile app

---

*For the latest updates and documentation, visit the [GitHub repository](https://github.com/getkushed/claude-code).*