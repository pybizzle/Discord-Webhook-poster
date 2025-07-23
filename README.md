# Discord Post Manager 🚀

A beautiful, feature-rich web application for creating, managing, and sending custom posts to Discord via webhooks. Perfect for server administrators, content creators, and anyone who needs to manage multiple Discord channels efficiently.

![Discord Webhook Poster](https://img.shields.io/badge/Discord-Post%20Manager-5865f2?style=for-the-badge&logo=discord&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

## ✨ Features

### 🔗 **Webhook Manager**
- Save multiple webhooks with descriptive names
- Add optional descriptions for better organization
- Test webhooks with one-click verification
- Edit and delete webhooks easily
- No more copying/pasting long webhook URLs

### ✏️ **Post Creation & Management**
- **Simple Messages**: Send plain text messages
- **Rich Embeds**: Create beautiful embedded messages with:
  - Custom titles and descriptions
  - Clickable URLs
  - Images and thumbnails
  - Custom colors
  - Live preview as you type
- Save posts as templates for reuse
- Edit and delete saved posts

### 🚀 **Quick Send**
- Send messages instantly without saving
- Select any saved webhook
- Perfect for one-off announcements

### 🎨 **User Experience**
- **Dark/Light Mode**: Toggle between themes
- **Responsive Design**: Works on desktop, tablet, and mobile
- **Live Preview**: See exactly how your message will look in Discord
- **Tabbed Interface**: Organized workflow with three main sections
- **Auto-switching**: Automatically switches tabs when editing
- **Auto-save**: Automatically saves to browser storage
- **Export/Import**: Backup and share your configurations

### 📁 **Data Management**
- **Auto-save**: Automatically saves to browser's localStorage
- **Export Options**:
  - Export all data (safe - URLs redacted)
  - Export all data with URLs (⚠️ includes actual webhook URLs)
  - Export webhooks only
  - Export posts only
- **Post Collections**: 
  - Import/export post collections for different servers
  - Quick template downloads (Gaming, Community, Business)
  - Replace or add to existing posts
- **.env File Support**: Store webhook URLs separately with custom naming
- **Security**: URLs redacted by default, optional full export available
- **Multi-Server Support**: Easy switching between different server configurations
- **Backup**: Create backups before major changes

### 📱 **Template System**
- **Minimal Examples**: Just 2 basic examples (simple message & rich embed)
- **Template Downloads**: Ready-to-use collections for different server types:
  - 🎮 Gaming Server templates
  - 👥 Community Server templates  
  - 💼 Business/Team templates
- **Custom Collections**: Import/export your own post collections
- **Server-Specific**: Switch between different post sets for different servers

## 🚀 Getting Started

### Prerequisites
- A web browser (Chrome, Firefox, Safari, Edge)
- Discord webhook URLs from your servers

### Installation

1. **Download the file**
   ```bash
   git clone https://github.com/yourusername/discord-post-manager.git
   cd discord-post-manager
   ```

2. **Open in browser**
   - Simply open `discord-post-manager.html` in your web browser
   - No server setup required - it's a standalone HTML file!

### Getting Discord Webhooks

1. Go to your Discord server settings
2. Navigate to **Integrations** → **Webhooks**
3. Click **New Webhook** or **Create Webhook**
4. Configure the webhook:
   - Set a name (e.g., "Announcements Bot")
   - Choose the channel
   - Optionally set an avatar
5. Copy the **Webhook URL**
6. Click **Save**

## 📖 Usage Guide

### Setting Up Webhooks

1. Open the **Webhook Manager** tab
2. Click **Add/Edit Webhook**
3. Fill in the details:
   - **Name**: A descriptive name (e.g., "Main Server - General")
   - **URL**: Your Discord webhook URL
   - **Description**: Optional note about the webhook's purpose
4. Click **Save Webhook**
5. Test it with the **Test Webhook** button

### Creating Posts

1. Go to the **Create Post** tab
2. Select a webhook from the dropdown
3. Enter your post details:
   - **Title**: For organization (not sent to Discord)
   - **Content**: Your message text
   - **Type**: Choose "Simple Message" or "Rich Embed"
4. For rich embeds, configure additional options:
   - Embed title, description, URLs
   - Images and thumbnails
   - Custom colors
5. Watch the live preview update as you type
6. Either **Save Post** for later use or **Send to Discord** immediately

### Managing Saved Posts

1. Visit the **Saved Posts** tab
2. **Browse Posts**: Click any post to select and preview it
3. **Preview Panel**: See exactly how your message will look in Discord
4. **Select Webhook**: Choose which webhook to send with in the preview panel
5. **Actions**: Edit, Send, or Delete the selected post

### Post Collections

#### Using Templates
1. **Download Templates**: Click Gaming, Community, or Business buttons for ready-made collections
2. **Import Templates**: Upload the downloaded JSON files to add posts to your collection
3. **Customize**: Edit the template posts to match your server's needs

#### Managing Collections
1. **Export Posts**: Save your current post collection as a JSON file
2. **Import Posts**: Load post collections from JSON files
3. **Replace vs Add**: Choose to replace all posts or add to existing ones
4. **Clear All**: Remove all posts except the basic examples

#### Multi-Server Workflow
1. **Export** your current server's posts before switching
2. **Clear All** to remove current posts
3. **Import** the new server's post collection
4. **Upload .env** file to restore webhook URLs for the new server

### Quick Send

Use the Quick Send section in the Create Post tab for one-off messages:
1. Select a webhook
2. Type your message
3. Click **Send Now**

### Data Management

#### Exporting Data
1. Go to the **Webhook Manager** tab
2. Use the **Backup & Share** section:
   - **Export All Data (Safe)**: Downloads posts and webhooks (URLs redacted for security)
   - **Export with URLs ⚠️**: Downloads with actual webhook URLs (use carefully!)
   - **Export Webhooks Only**: Downloads just webhook configurations
   - **Export Posts Only**: Downloads just your post templates
3. Files are saved as JSON with timestamp in filename

#### Using .env Files (Recommended)
1. **Download .env Template**: Creates a template with examples and current webhooks
2. **Customize the Names**: Use any names you want for your webhooks
3. **Add Your URLs**: Replace example URLs with your actual Discord webhook URLs
4. **Store Safely**: Keep your .env file secure and separate from shared exports
5. **Import Options**: When uploading, choose to create new webhooks or update existing ones

#### Importing Data
1. Click **Import Data** in the Webhook Manager tab
2. Select a previously exported JSON file
3. Data will be merged with existing content
4. **Restore URLs**: Upload your .env file to automatically restore webhook URLs

#### .env File Format
Your .env file can use **any names you want**! Examples:
```bash
# Discord Post Manager - Webhook URLs
# Use any descriptive names that make sense to you!

MAIN_SERVER_GENERAL=https://discord.com/api/webhooks/123456789/abcdef...
MY_PERSONAL_BOT=https://discord.com/api/webhooks/234567890/bcdefg...
WORK_PROJECT_UPDATES=https://discord.com/api/webhooks/345678901/cdefgh...
GAMING_CLAN_ANNOUNCEMENTS=https://discord.com/api/webhooks/456789012/defghi...
DEV_TESTING_CHANNEL=https://discord.com/api/webhooks/567890123/efghij...
COMMUNITY_WELCOME_BOT=https://discord.com/api/webhooks/678901234/fghijk...
```

**Rules:**
- Use any descriptive names you want (letters, numbers, underscores only)
- Names will be converted to "Title Case" when imported (DEV_TESTING → Dev Testing)
- No spaces in names (use underscores instead)
- Comments start with `#`
- Only valid Discord webhook URLs are accepted
- Add as many webhooks as you need!

#### Auto-save
- Data automatically saves to your browser's localStorage
- Persists between sessions (unless you clear browser data)
- No manual saving required

## 🎨 Customization

### Themes
Toggle between light and dark modes using the theme button in the top-right corner.

### Adding Custom Templates
Edit the `savedPosts` array in the JavaScript section to add your own default templates.

### Styling
Modify the CSS variables in the `:root` section to customize colors and appearance.

## 🔧 Technical Details

- **Frontend**: Pure HTML5, CSS3, and Vanilla JavaScript
- **Storage**: 
  - Auto-save to browser's localStorage
  - Export/Import via JSON files
  - .env file support for webhook URLs
  - In-memory during session
- **API**: Uses Discord's Webhook API
- **Security**: 
  - Webhook URLs redacted by default in exports
  - Optional full export with security warnings
  - .env files for separate URL management
- **File Formats**: JSON for data, .env for webhook URLs
- **Responsive**: Mobile-first CSS Grid and Flexbox layout
- **Accessibility**: Proper ARIA labels and keyboard navigation

## 🌟 Features in Detail

### Webhook Management
- **Centralized Storage**: All webhooks in one place
- **Smart Validation**: Ensures URLs are valid Discord webhooks
- **Quick Testing**: One-click webhook verification
- **Easy Organization**: Descriptive names and descriptions

### Message Types

#### Simple Messages
Perfect for quick announcements and casual messages.

#### Rich Embeds
Create professional-looking messages with:
- **Titles**: Optional clickable titles
- **Descriptions**: Formatted text with markdown support
- **Colors**: Custom embed border colors
- **Images**: Full-width images
- **Thumbnails**: Small images in the top-right
- **URLs**: Make the title clickable

### Live Preview
See exactly how your message will appear in Discord before sending, including:
- Text formatting
- Embed styling
- Image placement
- Color schemes

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Discord for their excellent webhook API
- The gaming community for inspiration on the template messages
- Contributors and users who provide feedback

## 📞 Support

If you encounter any issues or have questions:
1. Check the [Issues](https://github.com/pybizzle/Discord-Webhook-poster/issues) page
2. Create a new issue with detailed information
3. Include browser information and steps to reproduce

## 🔮 Future Features

- [x] Local storage persistence ✅
- [x] Export/Import configurations ✅
- [ ] Scheduled messages
- [ ] Webhook analytics
- [ ] Custom emoji support
- [ ] Message templates marketplace
- [ ] Bulk message sending
- [ ] Message history
- [ ] Cloud sync between devices
- [ ] Webhook rate limiting protection
- [ ] Message drafts and versioning

---

**Made with ❤️ for the Discord community**

*Star this repo if you find it useful! ⭐* 
