# Add AbletonOps to the Ableton project

Status checked 1 November 2026: the available project listing identifies a **local** project named Ableton, currently rooted at `E:\Data\AbletonProjects`. No ChatGPT cloud project named Ableton was returned. The available project tools do not expose editing its attached folders, so no connection has been made automatically.

## Attach the repository to the existing local project

1. In the desktop app, open **Projects**, then the **Ableton** project's menu.
2. Select **Edit project**.
3. Select **Add folder** and choose `E:\Data\GithubProjects\AbletonOps`.
4. Save/apply the change if the dialog offers that action. Start a new chat in Ableton and confirm that both folders are available.

Keep the current primary folder if music projects should remain the default. If future Git work should target AbletonOps by default, point to its folder in Edit project and choose **Make primary**.

[Official OpenAI project documentation](https://learn.chatgpt.com/docs/projects) describes multi-folder local projects and explains that Git operations use the primary repository. Adding a folder grants project chats file access; it is distinct from uploading a source snapshot or syncing an entire repository to the cloud.

## If you mean a separate ChatGPT cloud project

Open that project's **Sources** section and upload selected Markdown files, starting with README and the Move kit guide. Uploads are snapshots and must be refreshed after changes. Use a supported connected source if offered by your account. A Windows folder path alone does not connect a cloud project to the local repository. Nothing has been uploaded or pushed by this setup task.
