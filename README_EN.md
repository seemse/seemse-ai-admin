# Seemse AI Admin

> English Documentation | [中文文档](./README.md)

Deeply customized and developed based on **RuoYi AI Admin (若依AI管理系统)**, which in turn is built on the **Vben Admin framework**, featuring comprehensive permission management, system monitoring and other enterprise-grade functional modules.

Seemse AI is a complete artificial intelligence solution that includes backend services, admin panels, chat applications and other sub-projects, providing enterprises with comprehensive AI capability support.

## 🌐 Project Ecosystem

Seemse AI is a complete artificial intelligence solution that includes the following core projects:

### 📦 Core Projects
- **Backend Project** : [https://github.com/seemse/seemse_ai](https://github.com/seemse/seemse_ai) 
  - AI service backend built with Spring Boot + MyBatis Plus
  - Provides core API services for user management, AI model management, conversation processing
  - Supports multiple AI model integrations (OpenAI, Claude, Wenxin Yiyan, etc.)

- **Admin Panel** : [https://github.com/seemse/seemse-ai-admin](https://github.com/seemse/seemse-ai-admin)  
  - Enterprise-level admin backend based on Vue 3 + Ant Design Vue
  - Provides user management, system configuration, AI model configuration, data statistics
  - Supports enterprise features like permission management, system monitoring, log management

- **Chat Application Frontend** : [https://github.com/seemse/seemse-ai-web](https://github.com/seemse/seemse-ai-web)
  - Modern chat application based on Vue 3 + TypeScript
  - Supports multi-model conversations, history records, file uploads
  - Responsive design supporting PC and mobile access

### 🔗 Project Relationship Diagram
```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│  seemse-ai-web  │    │ seemse-ai-admin │    │  seemse_ai      │
│  (Chat Frontend)│    │  (Admin Panel)  │    │  (Backend)      │
└─────────────────┘    └─────────────────┘    └─────────────────┘
         │                       │                       │
         └───────────────────────┼───────────────────────┘
                                 │
                    ┌─────────────────┐
                    │   Users/Admins  │
                    │ (Unified User   │
                    │   System)       │
                    └─────────────────┘
```

### 🎯 Quick Navigation
| Project | Tech Stack | Main Features | Status |
|---------|------------|---------------|--------|
| seemse_ai | Spring Boot, MyBatis Plus, Redis | AI Services, User Management, Model Management | ✅ Stable |
| seemse-ai-admin | Vue 3, TypeScript, Ant Design Vue | Admin Panel, System Configuration | ✅ Stable |
| seemse-ai-web | Vue 3, TypeScript, Vite | Chat Application, AI Conversations | ✅ Stable |

## ✨ Features

- 🎯 **Modern Architecture**: Built with Vue 3 + TypeScript + Vite, adopting the latest frontend technology stack
- 🛠️ **Rich Components**: Integrated with Ant Design Vue component library, providing 50+ high-quality business components
- 🔐 **Permission Management**: Complete RBAC permission control system, supporting menu permissions, button permissions, and data permissions
- 📊 **System Monitoring**: Real-time system status monitoring, including online users, service monitoring, cache monitoring, etc.
- 📱 **Responsive Design**: Perfect adaptation to various device screens, supporting PC, tablet, and mobile access
- 🎨 **Theme Customization**: Support multiple theme switching and custom theme colors
- 🌍 **Internationalization**: Built-in internationalization solution with multi-language support
- ⚡ **High Performance**: Built with Vite, supporting hot module replacement for excellent development experience
- 📦 **Micro-frontend Architecture**: Support micro-frontend architecture for easy large project splitting and maintenance
- 🤖 **AI Capability Integration**: Deep integration of AI digital human, model management, knowledge base and other AI functional modules
- 📋 **Code Generation**: Built-in code generator, supporting rapid CRUD code generation
- 🔧 **Low-code Development**: Support form designer, flow designer and other low-code development tools

## 🚀 Tech Stack

### Frontend Technologies
- **Vue 3** - Progressive JavaScript framework
- **TypeScript** - Superset of JavaScript
- **Vite** - Next generation frontend build tool
- **Ant Design Vue** - Enterprise-class UI component library
- **Pinia** - Vue state management
- **Vue Router** - Official routing manager

### Development Tools
- **pnpm** - Fast, disk space efficient package manager
- **Turbo** - High-performance build system
- **ESLint** - Code quality checker
- **Prettier** - Code formatter
- **Husky** - Git hooks tool
- **Commitlint** - Git commit message linting
- **Lint-staged** - Pre-commit code checking

### Backend Integration
- **Spring Boot** - Backend service framework (requires backend project)
- **MyBatis Plus** - Data persistence layer framework
- **Redis** - Caching and session storage
- **MySQL** - Relational database

## 📋 Requirements

- **Node.js** >= 20.10.0
- **pnpm** >= 9.12.0

## 🛠️ Quick Start

### 1. Environment Preparation
Ensure your development environment meets the following requirements:
- Node.js >= 20.10.0 (Recommend using [nvm](https://github.com/nvm-sh/nvm) to manage Node versions)
- pnpm >= 9.12.0 (Install command: `npm install -g pnpm`)
- Git (For code version control)

### 2. Clone the project
```bash
# Clone the project code
git clone https://github.com/seemse/seemse-ai-admin
cd seemse-ai-admin
```

### 3. Install dependencies
```bash
# Install project dependencies
pnpm install

# If you encounter issues during installation, try clearing cache and reinstalling
# pnpm store prune && pnpm install
```

### 4. Start development server
```bash
# Start Ant Design Vue version development server
pnpm run dev:antd

# The application will start at http://localhost:3000
# Default username/password: admin/123456
```

### 5. Build for production
```bash
# Build production environment code
pnpm run build:antd

# Built files will be output to apps/web-antd/dist directory
```

### 6. Code quality checks
```bash
# Run code linting
pnpm run lint

# Run type checking
pnpm run check:type

# Run code formatting
pnpm run format
```

## 📝 Important Notes & Best Practices

### 🔧 Development Environment Configuration
1. **Node.js Version**: Please ensure you're using Node.js 20.10.0 or higher
2. **Package Manager**: This project uses pnpm, do not use npm or yarn
3. **Development Environment**: VS Code with relevant plugins is recommended
   - [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) - Vue 3 official plugin
   - [TypeScript Vue Plugin](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin) - TypeScript support
   - [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) - Code quality checking
   - [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) - Code formatting
4. **Browser Support**: Supports modern browsers, IE is not supported

### 🚀 Performance Optimization Suggestions
- Use `pnpm run build:analyze` to analyze build bundle size
- Import component libraries on demand to reduce bundle size
- Use Web Workers for complex computation tasks
- Enable HTTP/2 and Gzip compression to improve loading speed

### 🔒 Security Suggestions
- Regularly update dependency versions to fix security vulnerabilities
- Use HTTPS protocol for production deployment
- Configure appropriate CORS policies
- Perform strict validation and filtering of user input

### 📊 Monitoring & Logging
- Recommend integrating frontend monitoring tools (like Sentry)
- Configure appropriate log levels and output
- Monitor core performance metrics (FCP, LCP, FID, etc.)
- Set up error alerting mechanisms

## 📚 Project Structure

```
seemse-ai-admin/
├── apps/                    # Applications directory
│   ├── web-antd/           # Ant Design Vue version main application
│   │   ├── src/
│   │   │   ├── api/         # API layer (organized by business modules)
│   │   │   │   ├── aihuman/     # AI digital human related APIs
│   │   │   │   ├── core/        # Core functionality APIs (user, menu, permissions, etc.)
│   │   │   │   ├── monitor/     # System monitoring APIs
│   │   │   │   ├── operator/    # Operations related APIs (models, knowledge base, messages, etc.)
│   │   │   │   ├── system/      # System management APIs (department, role, dictionary, etc.)
│   │   │   │   └── workflow/    # Workflow related APIs
│   │   │   ├── components/  # Business components
│   │   │   ├── views/       # Page views (organized by business modules)
│   │   │   │   ├── _core/       # Core pages (login, profile, error pages, etc.)
│   │   │   │   ├── aihuman/     # AI digital human management
│   │   │   │   ├── dashboard/   # Dashboard (analytics, workspace)
│   │   │   │   ├── monitor/     # System monitoring (online users, operation logs, etc.)
│   │   │   │   ├── operator/    # Operations management (user management, model management, etc.)
│   │   │   │   └── system/      # System management (department management, role management, etc.)
│   │   │   └── utils/       # Utility functions
├── packages/               # Shared packages
│   ├── @core/             # Core package (components, directives, utilities, etc.)
│   ├── constants/         # Constants definition
│   ├── effects/           # Side effects handling (requests, storage, etc.)
│   ├── icons/             # Icon library
│   ├── locales/           # Internationalization
│   ├── preferences/       # Preference settings
│   ├── stores/            # State management (Pinia)
│   ├── styles/            # Style files (Tailwind CSS)
│   ├── types/             # Type definitions
│   └── utils/             # Utility functions
├── internal/              # Internal tools (build configuration, code checking, etc.)
└── scripts/               # Build scripts
```

---

**Seemse AI Admin - Making enterprise-level backend management simpler and more efficient!**