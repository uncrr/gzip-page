<script setup lang="ts">
import { useI18n } from 'vue-i18n'

const { locale } = useI18n()
</script>

<template>
  <div class="policy-page">
    <div class="container">
      <div class="policy-container">
        <div v-if="locale === 'zh-CN'" class="policy-content">
          <h1>Gzip Explorer — 隐私政策</h1>
          <p>最后更新日期：2025年12月17日</p>
          <h2>概述</h2>
          <p>
            本隐私页面描述了移动应用程序 <strong>Gzip Explorer</strong> 的数据实践。它是一款轻量级移动应用，其唯一运行行为是提取 <strong>.zip</strong> 代码项目归档，并在代码编辑器查看器和 markdown 渲染器中显示其文件。该应用不会收集、存储或传输个人数据，仅在设备上执行这些操作。
          </p>
          <h2>Gzip Explorer 不收集的内容</h2>
          <ul>
            <li>无个人标识符（姓名、电子邮件、电话号码）。</li>
            <li>
              无行为分析、页面查看跟踪或热图。
            </li>
            <li>
              无用于分析跟踪的 cookie 或本地存储。
            </li>
            <li>无用户账户、认证或配置文件存储。</li>
            <li>无向服务器传输用户提供数据的表单。</li>
            <li>
              从 `.zip` 归档提取的文件在设备上本地处理，且不会被应用上传。
            </li>
          </ul>
          <h2>为什么重要</h2>
          <p>
            最小化数据收集可降低风险并简化合规性。该应用有意避免添加任何（客户端或服务器）代码来捕获用户数据。
          </p>
          <h2>广告和第三方资源</h2>
          <p>
            该移动应用可能在应用开发者选择的地点显示广告。这些是非针对性广告，旨在支持开发，且不会用于构建配置文件或针对用户。
          </p>
          <p>
            如果未来贡献者添加第三方脚本或广告 SDK，必须获得批准并在本页面明确记录。
          </p>
          <h2>安全性和代码实践</h2>
          <ul>
            <li>
              不存在接受或存储 POST 用户数据的服务器端端点。
            </li>
            <li>
              所有应用文件处理（解压和文件渲染）均在设备上进行；应用不会将文件内容传输到远程服务器。
            </li>
            <li>
              在未审查且未在本页面明确记录的情况下，避免引入 SSR 端点或任何网络数据收集。
            </li>
            <li>
              编辑代码时遵循安全编码实践：在适用的地方验证输入，并避免类似 eval 的模式。
            </li>
          </ul>
          <h2>本政策的变更</h2>
          <p>
            如果应用将来更改为收集数据，本页面将更新，并在此明确记录变更。
          </p>
          <h2>联系方式</h2>
          <p>
            如果您对本隐私方法或 <strong>Gzip Explorer</strong> 的行为有疑问，请在此仓库中打开 issue 或添加 pull request 以建议对本文档的更改。
          </p>
          <footer style="margin-top:48px;font-size:0.9rem;color:#666;">
            &copy; 2025 Gzip Explorer. 保留所有权利。
          </footer>
        </div>
        <div v-else class="policy-content">
          <h1>Gzip Explorer — Privacy Policy</h1>
          <p>Last updated: December 17, 2025</p>
          <h2>Overview</h2>
          <p>
            This privacy page describes the data practices for the mobile
            application <strong>Gzip Explorer</strong>. It is a lightweight
            mobile app whose only runtime behavior is to extract <strong
              >.zip</strong
            > code project archives and display their files in a code editor
            viewer and markdown renderer. The app does not collect, store, or
            transmit personal data beyond what is required to perform these actions
            on-device.
          </p>
          <h2>What Gzip Explorer Does NOT Collect</h2>
          <ul>
            <li>No personal identifiers (names, emails, phone numbers).</li>
            <li>
              No behavioral analytics, page-view tracking, or heatmaps.
            </li>
            <li>
              No cookies or local storage used for tracking for analytics.
            </li>
            <li>No user accounts, authentication, or profile storage.</li>
            <li>No forms that transmit user-provided data to servers.</li>
            <li>
              Files extracted from `.zip` archives are processed locally
              on the device and are not uploaded by the app.
            </li>
          </ul>
          <h2>Why This Matters</h2>
          <p>
            Minimizing data collection reduces risk and simplifies
            compliance. The site purposefully avoids adding any code (client
            or server) that would capture user data.
          </p>
          <h2>Ads and Third-Party Resources</h2>
          <p>
            The mobile app may display ads in places selected by the app
            developer. These are non-targeted ads intended to support
            development and are not used to build profiles or target users.
          </p>
          <p>
            If any future contributor adds a third-party script or ad SDK,
            it must be approved and explicitly documented on this page.
          </p>
          <h2>Security & Code Practices</h2>
          <ul>
            <li>
              No server-side endpoints exist that accept or store POSTed
              user data.
            </li>
            <li>
              All app file processing (unzipping and file rendering)
              happens on-device; the app does not transmit file contents
              to remote servers.
            </li>
            <li>
              Avoid introducing SSR endpoints or any networked data
              collection without review and explicit documentation on this
              page.
            </li>
            <li>
              Follow secure coding practices when editing code: validate
              inputs where applicable and avoid eval-like patterns.
            </li>
          </ul>
          <h2>Changes to This Policy</h2>
          <p>
            If the site ever changes to collect data, this page will be
            updated and the change will be explicitly documented here.
          </p>
          <h2>Contact</h2>
          <p>
            If you have questions about this privacy approach or the
            behavior of <strong>Gzip Explorer</strong>, open an issue in
            this repository or add a pull request with suggested changes to
            this document.
          </p>
          <footer style="margin-top:48px;font-size:0.9rem;color:#666;">
            &copy; 2025 Gzip Explorer. All Rights are Reserved.
          </footer>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.policy-page {
  padding-top: 120px;
  padding-bottom: 80px;
  min-height: 100vh;
}

.policy-container {
  max-width: 800px;
  margin: 0 auto;
  background-color: var(--surface-color);
  border-radius: 20px;
  padding: 60px;
  box-shadow: var(--shadow);
}

.policy-content h1 {
  font-size: 48px;
  font-weight: 700;
  color: var(--text-primary);
  margin-bottom: 40px;
  text-align: center;
  background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.policy-content h2 {
  font-size: 24px;
  font-weight: 600;
  color: var(--text-primary);
  margin-top: 40px;
  margin-bottom: 20px;
  border-bottom: 2px solid var(--primary-color);
  padding-bottom: 8px;
}

.policy-content p {
  font-size: 16px;
  line-height: 1.6;
  color: var(--text-secondary);
  margin-bottom: 16px;
}

.policy-content ul {
  margin: 16px 0;
  padding-left: 20px;
}

.policy-content li {
  font-size: 16px;
  line-height: 1.6;
  color: var(--text-secondary);
  margin-bottom: 8px;
}

.policy-content a {
  color: var(--primary-color);
  text-decoration: none;
  transition: var(--transition);
}

.policy-content a:hover {
  text-decoration: underline;
}

.policy-content strong {
  color: var(--text-primary);
  font-weight: 600;
}

@media (max-width: 768px) {
  .policy-container {
    padding: 40px 20px;
  }

  .policy-content h1 {
    font-size: 36px;
  }

  .policy-content h2 {
    font-size: 20px;
  }

  .policy-content p,
  .policy-content li {
    font-size: 14px;
  }
}
</style>