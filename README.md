<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1180 610" width="100%" height="100%" style="background: #030712; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif; border-radius: 16px; overflow: hidden;">
  <defs>
    <linearGradient id="accentGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#7C3AED" />
      <stop offset="50%" stop-color="#22D3EE" />
      <stop offset="100%" stop-color="#10B981" />
    </linearGradient>

    <linearGradient id="asciiGrad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#22D3EE">
        <animate attributeName="stop-color" values="#22D3EE; #7C3AED; #22D3EE" dur="8s" repeatCount="indefinite" />
      </stop>
      <stop offset="100%" stop-color="#7C3AED">
        <animate attributeName="stop-color" values="#7C3AED; #10B981; #7C3AED" dur="8s" repeatCount="indefinite" />
      </stop>
    </linearGradient>

    <linearGradient id="borderGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="rgba(255,255,255,0.08)" />
      <stop offset="50%" stop-color="rgba(34,211,238,0.3)">
        <animate attributeName="offset" values="0; 1; 0" dur="6s" repeatCount="indefinite" />
      </stop>
      <stop offset="100%" stop-color="rgba(124,58,237,0.08)" />
    </linearGradient>

    <filter id="glow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="8" result="blur" />
      <feComposite in="SourceGraphic" in2="blur" operator="over" />
    </filter>
    
    <filter id="subtleGlow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="3" result="blur" />
      <feComposite in="SourceGraphic" in2="blur" operator="over" />
    </filter>

    <filter id="cardBlur">
      <feGaussianBlur stdDeviation="20" />
    </filter>

    <pattern id="noise" width="100" height="100" patternUnits="userSpaceOnUse">
      <filter id="noiseFilter">
        <feTurbulence type="fractalNoise" baseFrequency="0.80" numOctaves="3" stitchTiles="stitch" />
        <feColorMatrix type="matrix" values="1 0 0 0 0  0 1 0 0 0  0 0 1 0 0  0 0 0 0.04 0" />
      </filter>
      <rect width="100" height="100" filter="url(#noiseFilter)" fill="none" />
    </pattern>
  </defs>

  <rect width="1180" height="610" fill="#030712" />

  <g opacity="0.25">
    <circle cx="200" cy="150" r="180" fill="#7C3AED" filter="url(#cardBlur)">
      <animate attributeName="cx" values="200; 250; 200" dur="10s" repeatCount="indefinite" />
      <animate attributeName="cy" values="150; 200; 150" dur="10s" repeatCount="indefinite" />
    </circle>
    <circle cx="950" cy="450" r="220" fill="#22D3EE" filter="url(#cardBlur)">
      <animate attributeName="cx" values="950; 900; 950" dur="12s" repeatCount="indefinite" />
      <animate attributeName="cy" values="450; 380; 450" dur="12s" repeatCount="indefinite" />
    </circle>
    <circle cx="590" cy="300" r="150" fill="#10B981" filter="url(#cardBlur)">
      <animate attributeName="cy" values="300; 340; 300" dur="8s" repeatCount="indefinite" />
    </circle>
  </g>

  <rect width="1180" height="610" fill="url(#noise)" />

  <rect width="1180" height="4" fill="rgba(34, 211, 238, 0.08)" opacity="0.8">
    <animate attributeName="y" values="-10; 620; -10" dur="8s" repeatCount="indefinite" />
  </rect>

  <g fill="#F8FAFC" opacity="0.3">
    <circle cx="100" cy="100" r="1.5"><animate attributeName="cy" values="100;90;100" dur="4s" repeatCount="indefinite"/><animate attributeName="opacity" values="0.2;0.8;0.2" dur="4s" repeatCount="indefinite"/></circle>
    <circle cx="500" cy="80" r="1"><animate attributeName="cy" values="80;70;80" dur="5s" repeatCount="indefinite"/><animate attributeName="opacity" values="0.1;0.6;0.1" dur="5s" repeatCount="indefinite"/></circle>
    <circle cx="1080" cy="200" r="2"><animate attributeName="cy" values="200;185;200" dur="6s" repeatCount="indefinite"/><animate attributeName="opacity" values="0.3;0.9;0.3" dur="6s" repeatCount="indefinite"/></circle>
    <circle cx="80" cy="500" r="1"><animate attributeName="cy" values="500;480;500" dur="7s" repeatCount="indefinite"/></circle>
    <circle cx="600" cy="540" r="1.5"><animate attributeName="cy" values="540;520;540" dur="5s" repeatCount="indefinite"/></circle>
  </g>

  <rect x="20" y="20" width="1140" height="570" rx="16" fill="#0F172A" fill-opacity="0.45" stroke="url(#borderGrad)" stroke-width="1.5" style="backdrop-filter: blur(20px);" />

  <path d="M 21 21 L 1159 21 L 950 589 L 21 589 Z" fill="url(#accentGrad)" opacity="0.01" />

  <g transform="translate(0, 0)">
    <animateTransform attributeName="transform" type="translate" values="0,0; 0,-8; 0,0" dur="6s" repeatCount="indefinite" ease="ease-in-out" />
    
    <rect x="50" y="50" width="410" height="510" rx="12" fill="#090D16" fill-opacity="0.8" stroke="rgba(255,255,255,0.05)" stroke-width="1" />
    
    <circle cx="75" cy="70" r="5" fill="#EF4444" />
    <circle cx="91" cy="70" r="5" fill="#F59E0B" />
    <circle cx="107" cy="70" r="5" fill="#10B981" />
    <text x="130" y="75" fill="#94A3B8" font-size="11" letter-spacing="1.5" font-family="monospace">CORE_IDENTITY.SH</text>

    <rect x="51" y="85" width="408" height="474" fill="none" rx="2" />

    <g transform="translate(65, 120)" font-family="monospace" font-weight="bold" font-size="11" fill="url(#asciiGrad)" style="filter: drop-shadow(0 0 4px rgba(34,211,238,0.25));">
      <text x="10" y="20" fill="#22D3EE" font-size="13">&gt; cat cyber_avatar.asc</text>
      
      <g transform="translate(10, 45)">
        <text x="0" y="20" opacity="0">░▒▓██████████████████▓▒░<animate attributeName="opacity" values="0;1" begin="0.2s" fill="freeze" dur="0.2s"/></text>
        <text x="0" y="36" opacity="0">▒██████▀▀▀▀▀▀▀▀▀▀██████▒<animate attributeName="opacity" values="0;1" begin="0.4s" fill="freeze" dur="0.2s"/></text>
        <text x="0" y="52" opacity="0">████▀    ▄▄▄  ▄▄▄    ▀████<animate attributeName="opacity" values="0;1" begin="0.6s" fill="freeze" dur="0.2s"/></text>
        <text x="0" y="68" opacity="0">███▒    ▒▓█▓▒░▒▓█▓▒    ▒███<animate attributeName="opacity" values="0;1" begin="0.8s" fill="freeze" dur="0.2s"/></text>
        <text x="0" y="84" opacity="0">███     ▒▓█▓▒░▒▓█▓▒     ███<animate attributeName="opacity" values="0;1" begin="1.0s" fill="freeze" dur="0.2s"/></text>
        <text x="0" y="100" opacity="0">███░                    ░███<animate attributeName="opacity" values="0;1" begin="1.2s" fill="freeze" dur="0.2s"/></text>
        <text x="0" y="116" opacity="0">███▒    █▄        ▄█    ▒███<animate attributeName="opacity" values="0;1" begin="1.4s" fill="freeze" dur="0.2s"/></text>
        <text x="0" y="132" opacity="0">████▄    ▀████████▀    ▄████<animate attributeName="opacity" values="0;1" begin="1.6s" fill="freeze" dur="0.2s"/></text>
        <text x="0" y="148" opacity="0">▒██████▄▄        ▄▄██████▒<animate attributeName="opacity" values="0;1" begin="1.8s" fill="freeze" dur="0.2s"/></text>
        <text x="0" y="164" opacity="0">░▒▓██████████████████▓▒░<animate attributeName="opacity" values="0;1" begin="2.0s" fill="freeze" dur="0.2s"/></text>
        
        <g fill="#94A3B8" font-size="10" font-family="monospace" opacity="0.8">
          <text x="10" y="210" opacity="0">STATUS: ACTIVE<animate attributeName="opacity" values="0;1" begin="2.3s" fill="freeze" dur="0.3s"/></text>
          <text x="10" y="228" opacity="0">MODULE: BLUE_TEAM_CORE<animate attributeName="opacity" values="0;1" begin="2.5s" fill="freeze" dur="0.3s"/></text>
          <text x="10" y="246" opacity="0">THREAT_INT: OPERATIONAL<animate attributeName="opacity" values="0;1" begin="2.7s" fill="freeze" dur="0.3s"/></text>
        </g>
      </g>
    </g>

    <g transform="translate(75, 490)">
      <circle cx="10" cy="10" r="5" fill="#10B981" filter="url(#subtleGlow)">
        <animate attributeName="opacity" values="0.4;1;0.4" dur="2s" repeatCount="indefinite" />
      </circle>
      <text x="25" y="14" fill="#10B981" font-size="11" font-family="monospace" letter-spacing="1">SYSTEMSEC_SECURE // OK</text>
    </g>
  </g>

  <g transform="translate(490, 50)">
    <rect x="0" y="0" width="640" height="510" rx="12" fill="#090D16" fill-opacity="0.75" stroke="rgba(255,255,255,0.06)" stroke-width="1.5" />
    
    <path d="M 0 12 A 12 12 0 0 1 12 0 L 628 0 A 12 12 0 0 1 640 12 L 640 40 L 0 40 Z" fill="#0F172A" fill-opacity="0.9" />
    <circle cx="20" cy="20" r="6" fill="#EF4444" />
    <circle cx="40" cy="20" r="6" fill="#F59E0B" />
    <circle cx="60" cy="20" r="6" fill="#10B981" />
    <text x="85" y="24" fill="#94A3B8" font-size="12" font-family="monospace">anzarahmed@muet-cybersec:~</text>

    <g transform="translate(30, 75)">
      
      <g>
        <text x="0" y="20" fill="#94A3B8" font-size="16" font-family="monospace" font-weight="bold">Hi, I'm</text>
        <text x="75" y="20" fill="url(#accentGrad)" font-size="28" font-family="-apple-system, sans-serif" font-weight="900" style="filter: drop-shadow(0 2px 10px rgba(34,211,238,0.15));">Anzar Ahmed</text>
      </g>

      <g transform="translate(0, 55)">
        <text x="0" y="10" fill="#22D3EE" font-size="14" font-family="monospace">&gt;&gt;</text>
        
        <g font-size="16" font-family="monospace" font-weight="bold" fill="#F8FAFC">
          <g>
            <text x="30" y="10" opacity="0">
              Cyber Security Student
              <animate attributeName="opacity" values="0;1;1;0;0" keys="0;0.05;0.30;0.35;1" dur="10s" repeatCount="indefinite" />
            </text>
          </g>
          <g>
            <text x="30" y="10" opacity="0">
              Threat Hunter &amp; Incident Responder
              <animate attributeName="opacity" values="0;0;1;1;0;0" keys="0;0.35;0.40;0.65;0.70;1" dur="10s" repeatCount="indefinite" />
            </text>
          </g>
          <g>
            <text x="30" y="10" opacity="0">
              Blue Teaming &amp; Automation Developer
              <animate attributeName="opacity" values="0;0;1;1;0" keys="0;0.70;0.75;0.95;1" dur="10s" repeatCount="indefinite" />
            </text>
          </g>
        </g>
        
        <rect x="355" y="-5" width="8" height="18" fill="#22D3EE" opacity="1">
          <animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite" />
          <animate attributeName="x" values="225;225;350;350;345;345;225" keys="0;0.30;0.35;0.65;0.70;0.95;1" dur="10s" repeatCount="indefinite" />
        </rect>
      </g>

      <g transform="translate(0, 105)" font-size="13" font-family="monospace">
        <g opacity="0">
          <animate attributeName="opacity" to="1" begin="0.5s" fill="freeze" dur="0.4s" />
          <text x="0" y="20" fill="#94A3B8">Education:</text>
          <text x="110" y="20" fill="#F8FAFC">BS Cyber Security @ Mehran University (MUET)</text>
        </g>

        <g opacity="0">
          <animate attributeName="opacity" to="1" begin="0.9s" fill="freeze" dur="0.4s" />
          <text x="0" y="45" fill="#94A3B8">Focus:</text>
          <text x="110" y="45" fill="#F8FAFC">SIEM Engineering, Log Automation, Threat Hunting</text>
        </g>

        <g opacity="0">
          <animate attributeName="opacity" to="1" begin="1.3s" fill="freeze" dur="0.4s" />
          <text x="0" y="70" fill="#94A3B8">Recent Dev:</text>
          <text x="110" y="70" fill="#22D3EE">Phishing Detection Orchestrator (n8n + VirusTotal API)</text>
        </g>

        <g opacity="0">
          <animate attributeName="opacity" to="1" begin="1.7s" fill="freeze" dur="0.4s" />
          <text x="0" y="95" fill="#94A3B8">Location:</text>
          <text x="110" y="95" fill="#F8FAFC">Karachi, Pakistan</text>
        </g>
      </g>

      <g transform="translate(0, 235)">
        <text x="0" y="15" fill="#94A3B8" font-size="12" font-family="monospace" letter-spacing="1">PREF_STACK_AND_TOOLS:</text>

        <g transform="translate(0, 30)" font-family="sans-serif" font-size="11" font-weight="600">
          <g transform="translate(0, 0)">
            <rect x="0" y="0" width="70" height="26" rx="13" fill="#1E293B" stroke="rgba(34,211,238,0.2)" stroke-width="1" />
            <text x="35" y="17" fill="#F8FAFC" text-anchor="middle">Wazuh</text>
          </g>
          <g transform="translate(80, 0)">
            <rect x="0" y="0" width="80" height="26" rx="13" fill="#1E293B" stroke="rgba(124,58,237,0.2)" stroke-width="1" />
            <text x="40" y="17" fill="#F8FAFC" text-anchor="middle">Suricata</text>
          </g>
          <g transform="translate(170, 0)">
            <rect x="0" y="0" width="80" height="26" rx="13" fill="#1E293B" stroke="rgba(16,185,129,0.2)" stroke-width="1" />
            <text x="40" y="17" fill="#F8FAFC" text-anchor="middle">Fortinet</text>
          </g>
          <g transform="translate(260, 0)">
            <rect x="0" y="0" width="80" height="26" rx="13" fill="#1E293B" stroke="rgba(34,211,238,0.2)" stroke-width="1" />
            <text x="40" y="17" fill="#F8FAFC" text-anchor="middle">pfSense</text>
          </g>
          <g transform="translate(350, 0)">
            <rect x="0" y="0" width="115" height="26" rx="13" fill="#1E293B" stroke="rgba(124,58,237,0.2)" stroke-width="1" />
            <text x="57.5" y="17" fill="#F8FAFC" text-anchor="middle">n8n Workflow</text>
          </g>

          <g transform="translate(0, 36)">
            <rect x="0" y="0" width="75" height="26" rx="13" fill="#1E293B" stroke="rgba(16,185,129,0.2)" stroke-width="1" />
            <text x="37.5" y="17" fill="#F8FAFC" text-anchor="middle">Python</text>
          </g>
          <g transform="translate(85, 36)">
            <rect x="0" y="0" width="65" height="26" rx="13" fill="#1E293B" stroke="rgba(34,211,238,0.2)" stroke-width="1" />
            <text x="32.5" y="17" fill="#F8FAFC" text-anchor="middle">GNS3</text>
          </g>
          <g transform="translate(160, 36)">
            <rect x="0" y="0" width="80" height="26" rx="13" fill="#1E293B" stroke="rgba(124,58,237,0.2)" stroke-width="1" />
            <text x="40" y="17" fill="#F8FAFC" text-anchor="middle">Logstash</text>
          </g>
          <g transform="translate(250, 36)">
            <rect x="0" y="0" width="75" height="26" rx="13" fill="#1E293B" stroke="rgba(16,185,129,0.2)" stroke-width="1" />
            <text x="37.5" y="17" fill="#F8FAFC" text-anchor="middle">Docker</text>
          </g>
          <g transform="translate(335, 36)">
            <rect x="0" y="0" width="55" height="26" rx="13" fill="#1E293B" stroke="rgba(34,211,238,0.2)" stroke-width="1" />
            <text x="27.5" y="17" fill="#F8FAFC" text-anchor="middle">Git</text>
          </g>
          <g transform="translate(400, 36)">
            <rect x="0" y="0" width="65" height="26" rx="13" fill="#1E293B" stroke="rgba(124,58,237,0.2)" stroke-width="1" />
            <text x="32.5" y="17" fill="#F8FAFC" text-anchor="middle">Linux</text>
          </g>
        </g>
      </g>

      <g transform="translate(0, 365)">
        <line x1="0" y1="0" x2="580" y2="0" stroke="rgba(255,255,255,0.06)" stroke-width="1" />
        
        <g transform="translate(0, 18)">
          <g transform="translate(0,0)" style="cursor: pointer;">
            <rect x="0" y="0" width="30" height="30" rx="8" fill="#1E293B" stroke="rgba(34,211,238,0.2)" stroke-width="1"/>
            <path d="M15 7c-4.4 0-8 3.6-8 8 0 3.5 2.3 6.5 5.5 7.6.4.1.5-.2.5-.4V21c-2.2.5-2.7-1.1-2.7-1.1-.4-.9-.9-1.2-.9-1.2-.7-.5.1-.5.1-.5.8.1 1.2.8 1.2.8.7 1.3 1.9.9 2.3.7.1-.5.3-.9.5-1.1-1.8-.2-3.6-.9-3.6-4 0-.9.3-1.6.8-2.1-.1-.2-.4-1 .1-2.1 0 0 .7-.2 2.2.8.6-.2 1.3-.3 2-.3s1.4.1 2 .3c1.5-1 2.2-.8 2.2-.8.5 1.1.2 1.9.1 2.1.5.5.8 1.2.8 2.1 0 3.1-1.9 3.7-3.7 3.9.3.3.6.8.6 1.5v2.2c0 .2.1.5.6.4 3.2-1.1 5.5-4.1 5.5-7.6 0-4.4-3.6-8-8-8z" fill="#F8FAFC"/>
          </g>
          <g transform="translate(42,0)" style="cursor: pointer;">
            <rect x="0" y="0" width="30" height="30" rx="8" fill="#1E293B" stroke="rgba(124,58,237,0.2)" stroke-width="1"/>
            <path d="M11 9H9v6h2V9zm-1-2c.6 0 1-.4 1-1s-.4-1-1-1-1 .4-1 1 .4 1 1 1zm9 4.5c0-1.9-1-2.5-2.2-2.5-1 0-1.4.5-1.6.8V9h-2v6h2v-3.5c0-.2 0-.4.1-.5.2-.3.4-.7.9-.7.6 0 .8.5.8 1.2V15h2V11.5z" fill="#F8FAFC"/>
          </g>
          <g transform="translate(84,0)" style="cursor: pointer;">
            <rect x="0" y="0" width="30" height="30" rx="8" fill="#1E293B" stroke="rgba(16,185,129,0.2)" stroke-width="1"/>
            <path d="M9 10l6 4 6-4v8H9v-8zm6 2.5L9.6 9h10.8L15 12.5z" fill="#F8FAFC"/>
          </g>
          <text x="130" y="20" fill="#94A3B8" font-size="11" font-family="monospace">CONNECT_PROT: ESTABLISHED</text>
        </g>
      </g>

    </g>
  </g>
</svg>
