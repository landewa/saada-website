export default function Home() {
  return (
    <main style={styles.main}>
      <div style={styles.container}>

        {/* NAV */}
        <nav style={styles.nav}>
          <div style={styles.logoWrap}>
            <img src="/logo.png" alt="SAADA" style={styles.logo} />
            <span style={styles.brand}>SAADA Reserve</span>
          </div>

          <div style={styles.navLinks}>
            <a href="#about" style={styles.link}>About</a>
            <a href="#roadmap" style={styles.link}>Roadmap</a>
            <a href="/whitepaper.pdf" target="_blank" style={styles.link}>Whitepaper</a>
          </div>
        </nav>

        {/* HERO */}
        <section style={styles.hero}>
          <h1 style={styles.title}>
            Digital Reserve for the Future of Web3
          </h1>

          <p style={styles.subtitle}>
            Transparent. Secure. Built on Binance Smart Chain.
          </p>

          <div style={styles.ctaWrap}>
            <a href="/whitepaper.pdf" target="_blank" style={styles.primaryBtn}>
              Read Whitepaper
            </a>

            <a 
              href="https://t.me/saadareserve"
              target="_blank"
              style={styles.secondaryBtn}
            >
              Join Community
            </a>
          </div>
        </section>

        {/* CONTRACT */}
        <section style={styles.card}>
          <p style={styles.cardLabel}>Contract Address</p>
          <code style={styles.contract}>
            0x280DD55C468cc00AadD675fA030E9914EB3Cee70
          </code>
        </section>

        {/* ABOUT */}
        <section id="about" style={styles.section}>
          <h2 style={styles.sectionTitle}>About SAADA</h2>

          <p style={styles.text}>
            SAADA Reserve is a decentralized reserve protocol designed to 
            provide transparency, security, and long-term sustainability 
            within the Web3 ecosystem.
          </p>

          <div style={styles.grid}>
            <div style={styles.feature}>
              <h3>🔐 Secure</h3>
              <p>Immutable smart contract system on BSC</p>
            </div>

            <div style={styles.feature}>
              <h3>👁 Transparent</h3>
              <p>All transactions verifiable on-chain</p>
            </div>

            <div style={styles.feature}>
              <h3>🌱 Sustainable</h3>
              <p>Designed for long-term ecosystem growth</p>
            </div>
          </div>
        </section>

        {/* ROADMAP */}
        <section id="roadmap" style={styles.section}>
          <h2 style={styles.sectionTitle}>Roadmap</h2>

          <div style={styles.roadmap}>
            <div>
              <h4>Phase 1</h4>
              <p>Launch, Website, Community</p>
            </div>

            <div>
              <h4>Phase 2</h4>
              <p>Marketing, Liquidity, Partnerships</p>
            </div>

            <div>
              <h4>Phase 3</h4>
              <p>Utility, Expansion, Scaling</p>
            </div>
          </div>
        </section>

        {/* SOCIAL */}
        <section style={styles.social}>
          <a 
            href="https://x.com/LanDewa8zme/status/2071886373431500952?s=20"
            target="_blank"
            style={styles.link}
          >
            Twitter
          </a>

          <a 
            href="https://t.me/saadareserve"
            target="_blank"
            style={styles.link}
          >
            Telegram
          </a>
        </section>

        {/* FOOTER */}
        <footer style={styles.footer}>
          © {new Date().getFullYear()} SAADA Reserve. All rights reserved.
        </footer>

      </div>
    </main>
  );
}

const styles: any = {
  main: {
    background: "#050505",
    color: "#fff",
    minHeight: "100vh",
    fontFamily: "Arial, sans-serif"
  },

  container: {
    maxWidth: "1100px",
    margin: "0 auto",
    padding: "20px"
  },

  nav: {
    display: "flex",
    justifyContent: "space-between",
    alignItems: "center",
    marginBottom: "40px"
  },

  logoWrap: {
    display: "flex",
    alignItems: "center",
    gap: "10px"
  },

  logo: {
    width: "40px"
  },

  brand: {
    fontWeight: "bold"
  },

  navLinks: {
    display: "flex",
    gap: "20px"
  },

  link: {
    color: "#aaa",
    textDecoration: "none"
  },

  hero: {
    textAlign: "center",
    marginBottom: "50px"
  },

  title: {
    fontSize: "48px",
    fontWeight: "bold"
  },

  subtitle: {
    color: "#aaa",
    marginTop: "10px"
  },

  ctaWrap: {
    marginTop: "20px",
    display: "flex",
    justifyContent: "center",
    gap: "15px"
  },

  primaryBtn: {
    background: "#fff",
    color: "#000",
    padding: "12px 20px",
    borderRadius: "8px",
    textDecoration: "none",
    fontWeight: "bold"
  },

  secondaryBtn: {
    border: "1px solid #333",
    padding: "12px 20px",
    borderRadius: "8px",
    color: "#fff",
    textDecoration: "none"
  },

  card: {
    background: "#0f0f0f",
    padding: "20px",
    borderRadius: "10px",
    marginBottom: "40px",
    textAlign: "center"
  },

  cardLabel: {
    color: "#888",
    fontSize: "12px"
  },

  contract: {
    fontSize: "13px"
  },

  section: {
    marginBottom: "50px"
  },

  sectionTitle: {
    fontSize: "28px",
    marginBottom: "15px"
  },

  text: {
    color: "#aaa"
  },

  grid: {
    display: "flex",
    gap: "20px",
    marginTop: "20px",
    flexWrap: "wrap"
  },

  feature: {
    background: "#111",
    padding: "20px",
    borderRadius: "10px",
    flex: "1"
  },

  roadmap: {
    display: "flex",
    gap: "20px",
    flexWrap: "wrap"
  },

  social: {
    display: "flex",
    justifyContent: "center",
    gap: "20px",
    marginTop: "40px"
  },

  footer: {
    textAlign: "center",
    marginTop: "50px",
    color: "#666",
    fontSize: "12px"
  }
};
