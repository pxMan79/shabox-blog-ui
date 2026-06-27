<template>
  <footer class="footer">
    <div class="footer-info">
      <span class="copyright">© 2026 ShaBox. All Rights Reserved.</span>
      <div class="beian-records" aria-label="网站备案信息">
        <a
          class="beian-link"
          href="https://beian.miit.gov.cn/"
          target="_blank"
          rel="noopener noreferrer"
        >
          陕ICP备2026016278号-1
        </a>
        <span class="record-separator" aria-hidden="true">|</span>
        <a
          class="beian-link public-security-link"
          href="https://beian.mps.gov.cn/#/query/webSearch?code=61012602000100"
          target="_blank"
          rel="noreferrer"
        >
          <img class="beian-icon" src="/beian-icon.png" alt="公安备案图标" />
          <span>陕公网安备61012602000100号</span>
        </a>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  width: 100%;
  min-height: 72px;
  padding: 16px 0;
  color: var(--text-muted);
  background-color: var(--bg-card);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px); /* 毛玻璃+兼容 */
  border-top: 1px solid rgba(120, 134, 160, 0.14);
  display: flex;
  align-items: center; /* 文字垂直居中 */
  justify-content: center;
}

.footer-info {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 6px;
  width: 100%;
  padding: 0 16px;
  font-size: 12px;
  text-align: center;
}

.copyright {
  letter-spacing: 0.02em;
}

.beian-records {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  gap: 8px;
  line-height: 1.5;
}

.beian-link {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  color: inherit;
  text-decoration: none; /* 去掉下划线 */
  transition: color 0.3s;
  white-space: nowrap;
}

.public-security-link {
  font-variant-numeric: tabular-nums;
}

.beian-icon {
  width: 16px;
  height: 16px;
  object-fit: contain;
  flex-shrink: 0;
}

.record-separator {
  color: color-mix(in srgb, var(--text-muted) 55%, transparent);
}

.beian-link:hover {
  color: #0f5aa6;
  text-decoration: underline;
  text-underline-offset: 3px;
}

@media (max-width: 767px) {
  .record-separator {
    display: none;
  }

  .beian-records {
    flex-direction: column;
    gap: 4px;
  }
}

@media (min-width: 768px) {
  .footer-info {
    font-size: 13px;
  }
}
</style>
