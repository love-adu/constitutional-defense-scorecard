import React, { useEffect, useMemo, useState } from "react";

const PILLARS = [
  { key: "purse", label: "Power of the purse" },
  { key: "trade", label: "Trade authority" },
  { key: "emergency", label: "Emergency powers" },
  { key: "war", label: "War powers" },
  { key: "troops", label: "Domestic troop deployment" },
  { key: "elections", label: "Election authority" },
  { key: "oversight", label: "Oversight & subpoena authority" },
  { key: "thirdterm", label: "Presidential third term" },
];

function ev(type, title, date, sourceLabel, url = "") {
  return { type, title, date, sourceLabel, url };
}

function commonsPhoto(filename, width = 360) {
  // Reliable hotlink to Wikimedia-hosted image via Commons.
  return `https://commons.wikimedia.org/wiki/Special:FilePath/${encodeURIComponent(
    filename
  )}?width=${width}`;
}

const gradeRank = { A: 1, B: 2, C: 3, D: 4, F: 5 };

function trafficForGrade(g) {
  if (g === "A" || g === "B") return { label: "Green", cls: "good" };
  if (g === "C") return { label: "Yellow", cls: "mid" };
  return { label: "Red", cls: "bad" };
}

function gradeDotClass(g) {
  if (g === "A" || g === "B") return "gA";
  if (g === "C") return "gC";
  return "gF";
}

const membersSeed = [
  {
    id: "jj",
    name: "Rep. Jim Jordan",
    wikiUrl: "https://en.wikipedia.org/wiki/Jim_Jordan_(American_politician)",
    photoUrl: commonsPhoto("Jim Jordan official photo, 114th Congress.jpg"),
    chamber: "House",
    state: "OH",
    priority: false,
    grade: "F",
    framing:
      "Consistent pattern of enabling executive overreach and undermining congressional checks.",
    pillars: {
      purse: {
        status: "bad",
        indicator:
          "Backed measures that weaken Congress’s ability to control spending and enforce appropriations limits.",
        evidence: [
          ev(
            "Vote",
            "Voted to advance a package reducing enforceable guardrails on appropriations oversight",
            "2026-01-14",
            "House Roll Call",
            "https://clerk.house.gov/Votes"
          ),
        ],
      },
      trade: {
        status: "bad",
        indicator:
          "Supported broad delegation of trade authority without strong oversight hooks.",
        evidence: [
          ev(
            "Statement",
            "Public comments favoring expanded executive flexibility on trade powers",
            "2025-12-18",
            "Press availability",
            "https://www.congress.gov/"
          ),
        ],
      },
      emergency: {
        status: "bad",
        indicator:
          "Supported expanding emergency authorities while opposing meaningful congressional review mechanisms.",
        evidence: [
          ev(
            "Cosponsor",
            "Co-sponsored legislation expanding emergency discretion with limited congressional constraints",
            "2026-01-06",
            "Bill sponsor list",
            "https://www.congress.gov/"
          ),
        ],
      },
      war: {
        status: "bad",
        indicator:
          "Opposed reforms that would require clearer congressional authorization for major uses of force.",
        evidence: [
          ev(
            "Vote",
            "Voted against AUMF reform resolution strengthening Congress’s role",
            "2026-02-02",
            "House Roll Call",
            "https://clerk.house.gov/Votes"
          ),
        ],
      },
      troops: {
        status: "bad",
        indicator:
          "Backed broad executive discretion for domestic deployments without firm Article I safeguards.",
        evidence: [
          ev(
            "Vote",
            "Voted against constraints on domestic troop deployment authorities",
            "2026-01-22",
            "House Roll Call",
            "https://clerk.house.gov/Votes"
          ),
        ],
      },
      elections: {
        status: "bad",
        indicator:
          "Supported positions that blur Congress’s role in safeguarding elections from executive interference.",
        evidence: [
          ev(
            "Statement",
            "Statement downplaying congressional guardrails on federal election administration",
            "2026-01-28",
            "Congressional Record (excerpt)",
            "https://www.congress.gov/congressional-record"
          ),
        ],
      },
      oversight: {
        status: "bad",
        indicator:
          "Pushed oversight selectively and opposed enforcement tools that strengthen Congress institutionally.",
        evidence: [
          ev(
            "Vote",
            "Voted against subpoena enforcement resources and institutional oversight capacity",
            "2026-02-04",
            "House Roll Call",
            "https://clerk.house.gov/Votes"
          ),
        ],
      },
      thirdterm: {
        status: "bad",
        indicator:
          "Did not take qualifying public steps to reject third-term normalization efforts during the scoring window.",
        evidence: [
          ev(
            "—",
            "No qualifying, verifiable action recorded in this period",
            "2026-02-18",
            "Scorecard note",
            ""
          ),
        ],
      },
    },
  },
  {
    id: "sc",
    name: "Sen. Susan Collins",
    wikiUrl: "https://en.wikipedia.org/wiki/Susan_Collins",
    photoUrl: commonsPhoto("Senator Susan Collins 2014 official portrait.jpg"),
    chamber: "Senate",
    state: "ME",
    priority: false,
    grade: "A",
    framing:
      "Consistently supports institutional checks and clear Article I guardrails across multiple pillars.",
    pillars: {
      purse: {
        status: "good",
        indicator:
          "Took actions reinforcing Congress’s spending authority and opposing unilateral executive impoundment.",
        evidence: [
          ev(
            "Letter",
            "Signed letter emphasizing congressional control of appropriations",
            "2026-01-20",
            "Public letter",
            "https://www.congress.gov/"
          ),
          ev(
            "Vote",
            "Voted for enforcement mechanisms protecting appropriations limits",
            "2026-01-12",
            "Senate Roll Call",
            "https://www.senate.gov/legislative/votes.htm"
          ),
        ],
      },
      trade: {
        status: "good",
        indicator:
          "Supported trade authorities with reporting requirements and congressional review provisions.",
        evidence: [
          ev(
            "Vote",
            "Voted for trade reporting and review amendments",
            "2026-01-30",
            "Senate Roll Call",
            "https://www.senate.gov/legislative/votes.htm"
          ),
        ],
      },
      emergency: {
        status: "good",
        indicator:
          "Backed limits on emergency declarations and clearer congressional termination pathways.",
        evidence: [
          ev(
            "Cosponsor",
            "Co-sponsored emergency powers reform with automatic congressional review",
            "2026-01-08",
            "Bill sponsor list",
            "https://www.congress.gov/"
          ),
        ],
      },
      war: {
        status: "good",
        indicator:
          "Supported requiring congressional authorization for significant uses of force.",
        evidence: [
          ev(
            "Cosponsor",
            "Co-sponsored AUMF reform resolution strengthening Congress’s war powers role",
            "2026-02-02",
            "Bill sponsor list",
            "https://www.congress.gov/"
          ),
        ],
      },
      troops: {
        status: "good",
        indicator:
          "Supported statutory guardrails for domestic deployments and clear reporting.",
        evidence: [
          ev(
            "Vote",
            "Voted for domestic deployment reporting/limits amendment",
            "2026-01-25",
            "Senate Roll Call",
            "https://www.senate.gov/legislative/votes.htm"
          ),
        ],
      },
      elections: {
        status: "good",
        indicator:
          "Supported election protection guardrails and rejected executive interference narratives.",
        evidence: [
          ev(
            "Statement",
            "Statement entered into the Congressional Record supporting election integrity guardrails",
            "2026-01-28",
            "Congressional Record",
            "https://www.congress.gov/congressional-record"
          ),
        ],
      },
      oversight: {
        status: "good",
        indicator:
          "Backed subpoena enforcement and institutional oversight capacity, not just partisan investigations.",
        evidence: [
          ev(
            "Vote",
            "Voted for subpoena enforcement resources",
            "2026-01-09",
            "Senate Roll Call",
            "https://www.senate.gov/legislative/votes.htm"
          ),
        ],
      },
      thirdterm: {
        status: "good",
        indicator:
          "Took qualifying public steps rejecting any normalization of a presidential third term.",
        evidence: [
          ev(
            "Statement",
            "Public statement rejecting third-term efforts as unconstitutional",
            "2026-02-10",
            "Press statement",
            "https://www.congress.gov/"
          ),
        ],
      },
    },
  },
  {
    id: "lm",
    name: "Sen. Lisa Murkowski",
    wikiUrl: "https://en.wikipedia.org/wiki/Lisa_Murkowski",
    photoUrl: commonsPhoto("Lisa Murkowski official photo.jpg"),
    chamber: "Senate",
    state: "AK",
    priority: false,
    grade: "A",
    framing:
      "Strong record of defending Congress’s role on spending, emergencies, and oversight.",
    pillars: {
      purse: {
        status: "good",
        indicator:
          "Supported measures reinforcing Congress’s spending authority and budget enforcement.",
        evidence: [
          ev(
            "Vote",
            "Voted to protect appropriations authority from unilateral executive override",
            "2026-01-12",
            "Senate Roll Call",
            "https://www.senate.gov/legislative/votes.htm"
          ),
        ],
      },
      trade: {
        status: "mid",
        indicator:
          "Mixed record: supported some reporting requirements but also backed broader delegation in one key vote.",
        evidence: [
          ev(
            "Vote",
            "Voted for trade transparency amendment",
            "2026-01-30",
            "Senate Roll Call",
            "https://www.senate.gov/legislative/votes.htm"
          ),
          ev(
            "Vote",
            "Voted against stronger congressional disapproval mechanism in trade authority",
            "2026-02-06",
            "Senate Roll Call",
            "https://www.senate.gov/legislative/votes.htm"
          ),
        ],
      },
      emergency: {
        status: "good",
        indicator:
          "Supported emergency powers reform that strengthens congressional review and termination.",
        evidence: [
          ev(
            "Cosponsor",
            "Co-sponsored emergency powers reform bill",
            "2026-01-08",
            "Bill sponsor list",
            "https://www.congress.gov/"
          ),
        ],
      },
      war: {
        status: "good",
        indicator:
          "Supported clearer authorization requirements for major uses of force.",
        evidence: [
          ev(
            "Vote",
            "Voted for AUMF reform resolution",
            "2026-02-02",
            "Senate Roll Call",
            "https://www.senate.gov/legislative/votes.htm"
          ),
        ],
      },
      troops: {
        status: "mid",
        indicator:
          "No qualifying action recorded in the scoring window (candidate for future indicators).",
        evidence: [
          ev(
            "—",
            "No qualifying, verifiable action recorded in this period",
            "2026-02-18",
            "Scorecard note",
            ""
          ),
        ],
      },
      elections: {
        status: "good",
        indicator:
          "Backed election guardrails and supported congressional role in election protection.",
        evidence: [
          ev(
            "Vote",
            "Voted for election safeguard provisions",
            "2026-01-19",
            "Senate Roll Call",
            "https://www.senate.gov/legislative/votes.htm"
          ),
        ],
      },
      oversight: {
        status: "good",
        indicator:
          "Supported oversight enforcement tools and institutional capacity.",
        evidence: [
          ev(
            "Vote",
            "Voted for subpoena enforcement resources",
            "2026-01-09",
            "Senate Roll Call",
            "https://www.senate.gov/legislative/votes.htm"
          ),
        ],
      },
      thirdterm: {
        status: "good",
        indicator:
          "Supported clear constitutional norms against a third term.",
        evidence: [
          ev(
            "Statement",
            "Public statement opposing third-term normalization",
            "2026-02-10",
            "Press statement",
            "https://www.congress.gov/"
          ),
        ],
      },
    },
  },
  {
    id: "tt",
    name: "Sen. Thom Tillis",
    wikiUrl: "https://en.wikipedia.org/wiki/Thom_Tillis",
    photoUrl: commonsPhoto("Sen. Thom Tillis official photo.jpg"),
    chamber: "Senate",
    state: "NC",
    priority: false,
    grade: "C",
    framing:
      "Middle-of-the-pack: some oversight and war powers support, but inconsistency on emergencies and spending guardrails.",
    pillars: {
      purse: {
        status: "mid",
        indicator:
          "Supported some appropriations guardrails, but did not consistently back enforcement mechanisms.",
        evidence: [
          ev(
            "Vote",
            "Voted for baseline appropriations protections",
            "2026-01-12",
            "Senate Roll Call",
            "https://www.senate.gov/legislative/votes.htm"
          ),
          ev(
            "Vote",
            "Voted against a stronger impoundment enforcement provision",
            "2026-02-01",
            "Senate Roll Call",
            "https://www.senate.gov/legislative/votes.htm"
          ),
        ],
      },
      trade: {
        status: "mid",
        indicator: "No clear qualifying action recorded in the scoring window.",
        evidence: [
          ev(
            "—",
            "No qualifying, verifiable action recorded in this period",
            "2026-02-18",
            "Scorecard note",
            ""
          ),
        ],
      },
      emergency: {
        status: "bad",
        indicator:
          "Supported a key expansion of emergency discretion without automatic congressional review.",
        evidence: [
          ev(
            "Vote",
            "Voted for emergency expansion measure",
            "2025-12-05",
            "Senate Roll Call",
            "https://www.senate.gov/legislative/votes.htm"
          ),
        ],
      },
      war: {
        status: "good",
        indicator:
          "Supported AUMF reform and clearer congressional authorization requirements.",
        evidence: [
          ev(
            "Cosponsor",
            "Co-sponsored AUMF reform resolution",
            "2026-02-02",
            "Bill sponsor list",
            "https://www.congress.gov/"
          ),
        ],
      },
      troops: {
        status: "mid",
        indicator:
          "No qualifying action recorded in the scoring window (candidate for future indicators).",
        evidence: [
          ev(
            "—",
            "No qualifying, verifiable action recorded in this period",
            "2026-02-18",
            "Scorecard note",
            ""
          ),
        ],
      },
      elections: {
        status: "mid",
        indicator:
          "Mixed: supported one guardrail but did not take additional qualifying actions.",
        evidence: [
          ev(
            "Vote",
            "Voted for a narrow election safeguard amendment",
            "2026-01-19",
            "Senate Roll Call",
            "https://www.senate.gov/legislative/votes.htm"
          ),
        ],
      },
      oversight: {
        status: "good",
        indicator:
          "Backed subpoena enforcement and oversight capacity in at least one key vote.",
        evidence: [
          ev(
            "Vote",
            "Voted for subpoena enforcement resources",
            "2026-01-09",
            "Senate Roll Call",
            "https://www.senate.gov/legislative/votes.htm"
          ),
        ],
      },
      thirdterm: {
        status: "mid",
        indicator: "No qualifying action recorded in the scoring window.",
        evidence: [
          ev(
            "—",
            "No qualifying, verifiable action recorded in this period",
            "2026-02-18",
            "Scorecard note",
            ""
          ),
        ],
      },
    },
  },
];

function GradeBadge({ grade, mode }) {
  const traffic = trafficForGrade(grade);
  const label = mode === "letters" ? grade : traffic.label;
  return (
    <span className="grade">
      <span className={`dotg ${gradeDotClass(grade)}`} />
      <span className="mono">{label}</span>
    </span>
  );
}

function PillarChip({ status, label }) {
  return <span className={`chip ${status}`}>{label}</span>;
}

export default function App() {
  const [view, setView] = useState("home");
  const [scaleMode, setScaleMode] = useState("letters");
  const [selectedId, setSelectedId] = useState(null);

  const [q, setQ] = useState("");
  const [chamber, setChamber] = useState("all");
  const [state, setState] = useState("all");
  const [priority, setPriority] = useState("all");
  const [sort, setSort] = useState("grade");

  const members = useMemo(() => membersSeed, []);

  const states = useMemo(() => {
    return Array.from(new Set(members.map((m) => m.state))).sort();
  }, [members]);

  const selected = useMemo(() => {
    return members.find((m) => m.id === selectedId) || null;
  }, [members, selectedId]);

  const filtered = useMemo(() => {
    const qq = q.trim().toLowerCase();
    let list = members.slice();

    if (qq) {
      list = list.filter(
        (m) =>
          m.name.toLowerCase().includes(qq) || m.state.toLowerCase().includes(qq)
      );
    }

    if (chamber !== "all") list = list.filter((m) => m.chamber === chamber);
    if (state !== "all") list = list.filter((m) => m.state === state);
    if (priority === "priority") list = list.filter((m) => m.priority);

    if (sort === "grade") {
      list.sort(
        (a, b) =>
          (gradeRank[a.grade] || 99) - (gradeRank[b.grade] || 99) ||
          a.name.localeCompare(b.name)
      );
    } else if (sort === "name") {
      list.sort((a, b) => a.name.localeCompare(b.name));
    } else if (sort === "state") {
      list.sort((a, b) => (a.state + a.name).localeCompare(b.state + b.name));
    }

    return list;
  }, [members, q, chamber, state, priority, sort]);

  useEffect(() => {
    const applyHash = () => {
      const h = window.location.hash || "";
      if (h.startsWith("#member=")) {
        const id = decodeURIComponent(h.split("=")[1] || "");
        setSelectedId(id);
        setView("detail");
      } else if (h === "#methodology") {
        setView("method");
      } else if (h === "#about") {
        setView("about");
      } else {
        setView("home");
      }
    };

    applyHash();
    window.addEventListener("hashchange", applyHash);
    return () => window.removeEventListener("hashchange", applyHash);
  }, []);

  function openMember(id) {
    window.location.hash = `member=${encodeURIComponent(id)}`;
  }

  async function shareOrCopy(url, title) {
    try {
      if (navigator.share) {
        await navigator.share({ title, url });
        toast("Shared.");
      } else {
        await navigator.clipboard.writeText(url);
        toast("Link copied.");
      }
    } catch {
      try {
        await navigator.clipboard.writeText(url);
        toast("Link copied.");
      } catch {
        toast("Couldn’t share automatically.");
      }
    }
  }

  function toast(msg) {
    const t = document.getElementById("toast");
    if (!t) return;
    t.textContent = msg;
    t.style.display = "block";
    window.clearTimeout(window.__toastTimer);
    window.__toastTimer = window.setTimeout(() => (t.style.display = "none"), 1800);
  }

  function goHome() {
    window.location.hash = "";
  }

  const lastUpdated = "February 18, 2026";

  return (
    <div className="page">
      <style>{css}</style>

      <header className="header">
        <div className="wrap topbar">
          <div className="brand" onClick={goHome} role="button" tabIndex={0}>
            <span className="dot" />
            <div>
              Constitutional Defense Scorecard <span className="muted">(Mock)</span>
            </div>
          </div>
          <nav className="nav">
            <button
              className={`navbtn ${view === "home" ? "active" : ""}`}
              onClick={() => (window.location.hash = "")}
            >
              Scorecard
            </button>
            <button
              className={`navbtn ${view === "method" ? "active" : ""}`}
              onClick={() => (window.location.hash = "methodology")}
            >
              Methodology
            </button>
            <button
              className={`navbtn ${view === "about" ? "active" : ""}`}
              onClick={() => (window.location.hash = "about")}
            >
              About
            </button>
          </nav>
        </div>
      </header>

      <main className="wrap main">
        {view === "home" && (
          <section>
            <div className="hero">
              <h1>Who is defending Congress’s Article I powers?</h1>
              <p>
                This scorecard tracks public, binary, verifiable actions showing whether
                Republican Members of Congress defend or abandon Congress’s constitutional
                authority in the face of executive overreach.
              </p>
              <div className="meta">
                <span className="pill">
                  Last updated: <strong>{lastUpdated}</strong>
                </span>
                <span className="pill">
                  Cadence: <strong>Monthly / Quarterly</strong>
                </span>
                <span className="pill">
                  Grades: <strong>A–F</strong> (or green/yellow/red)
                </span>
              </div>

              <div className="controls">
                <div className="control">
                  <label>Search</label>
                  <input
                    value={q}
                    onChange={(e) => setQ(e.target.value)}
                    placeholder="Name or state (e.g., Jordan, AK)"
                  />
                </div>

                <div className="control">
                  <label>Chamber</label>
                  <select value={chamber} onChange={(e) => setChamber(e.target.value)}>
                    <option value="all">All</option>
                    <option value="Senate">Senate</option>
                    <option value="House">House</option>
                  </select>
                </div>

                <div className="control">
                  <label>State</label>
                  <select value={state} onChange={(e) => setState(e.target.value)}>
                    <option value="all">All</option>
                    {states.map((s) => (
                      <option key={s} value={s}>
                        {s}
                      </option>
                    ))}
                  </select>
                </div>

                <div className="control">
                  <label>Priority races</label>
                  <select
                    value={priority}
                    onChange={(e) => setPriority(e.target.value)}
                  >
                    <option value="all">All</option>
                    <option value="priority">Priority only</option>
                  </select>
                </div>

                <div className="control">
                  <label>Sort</label>
                  <select value={sort} onChange={(e) => setSort(e.target.value)}>
                    <option value="grade">Grade (best to worst)</option>
                    <option value="name">Name (A–Z)</option>
                    <option value="state">State</option>
                  </select>
                </div>
              </div>

              <div className="row">
                <div className="muted small">
                  Click a member for a pillar-by-pillar breakdown (votes, cosponsorships,
                  letters, Congressional Record statements).
                </div>
                <div className="rowBtns">
                  <button
                    className="btn secondary"
                    onClick={() =>
                      setScaleMode((m) => (m === "letters" ? "traffic" : "letters"))
                    }
                  >
                    Toggle: A–F / Traffic light
                  </button>
                  <button
                    className="btn"
                    onClick={() =>
                      shareOrCopy(
                        `${window.location.href.split("#")[0]}#scorecard`,
                        "Constitutional Defense Scorecard"
                      )
                    }
                  >
                    Share scorecard
                  </button>
                </div>
              </div>
            </div>

            <div className="panel">
              <div className="tableWrap">
                <table>
                  <thead>
                    <tr>
                      <th style={{ width: "28%" }}>Member</th>
                      <th style={{ width: "10%" }}>State</th>
                      <th style={{ width: "12%" }}>Chamber</th>
                      <th style={{ width: "16%" }}>Overall</th>
                      <th>Pillar snapshot</th>
                    </tr>
                  </thead>
                  <tbody>
                    {filtered.length === 0 ? (
                      <tr>
                        <td colSpan={5} className="muted" style={{ padding: 18 }}>
                          No members match your filters.
                        </td>
                      </tr>
                    ) : (
                      filtered.map((m) => (
                        <tr key={m.id} className="clickable" onClick={() => openMember(m.id)}>
                          <td>
                            <div className="memberCell">
                              <a href={m.wikiUrl} target="_blank" rel="noreferrer" aria-label={`${m.name} Wikipedia`}>
                                <img
                                  className="avatar"
                                  src={m.photoUrl}
                                  alt={m.name}
                                  loading="lazy"
                                />
                              </a>
                              <div>
                                <strong>{m.name}</strong>{" "}
                                {m.priority && <span className="tag">PRIORITY</span>}
                              </div>
                            </div>
                          </td>
                          <td>{m.state}</td>
                          <td>{m.chamber}</td>
                          <td>
                            <GradeBadge grade={m.grade} mode={scaleMode} />
                          </td>
                          <td>
                            <div className="chips">
                              {[
                                { k: "purse", short: "Purse" },
                                { k: "emergency", short: "Emergency" },
                                { k: "war", short: "War" },
                                { k: "oversight", short: "Oversight" },
                              ].map(({ k, short }) => (
                                <PillarChip
                                  key={k}
                                  status={m.pillars?.[k]?.status || "mid"}
                                  label={short}
                                />
                              ))}
                            </div>
                          </td>
                        </tr>
                      ))
                    )}
                  </tbody>
                </table>
              </div>
            </div>
          </section>
        )}

        {view === "detail" && selected && (
          <section>
            <div className="row topRow">
              <button className="btn secondary" onClick={() => (window.location.hash = "")}>
                ← Back to scorecard
              </button>
              <div className="rowBtns">
                <button
                  className="btn secondary"
                  onClick={() =>
                    shareOrCopy(
                      `${window.location.href.split("#")[0]}#member=${encodeURIComponent(
                        selected.id
                      )}`,
                      `${selected.name} — Constitutional Defense Scorecard`
                    )
                  }
                >
                  Share member
                </button>
              </div>
            </div>

            <div className="detailGrid">
              <div className="card">
                <div className="cardHead">
                  <div className="nameBlock">
                    <a href={selected.wikiUrl} target="_blank" rel="noreferrer" aria-label={`${selected.name} Wikipedia`}>
                      <img
                        className="avatar lg"
                        src={selected.photoUrl}
                        alt={selected.name}
                        loading="lazy"
                      />
                    </a>
                    <div>
                      <h2 style={{ margin: 0 }}>{selected.name}</h2>
                      <div className="muted small" style={{ marginTop: 2 }}>
                        <a href={selected.wikiUrl} target="_blank" rel="noreferrer">
                          Wikipedia profile
                        </a>
                      </div>
                    </div>
                  </div>
                  <GradeBadge grade={selected.grade} mode={scaleMode} />
                </div>
                <div className="muted">
                  {selected.chamber} • {selected.state}
                  {selected.priority ? " • Priority race" : ""}
                </div>

                <div className="kv">
                  <div>Overall framing</div>
                  <div>{selected.framing}</div>
                  <div>What we score</div>
                  <div className="muted">
                    Public, binary, verifiable actions (votes, cosponsorship, letters,
                    formal statements).
                  </div>
                  <div>Why it matters</div>
                  <div className="muted">
                    Congress can’t defend its authority if its members choose not to use it.
                  </div>
                </div>
              </div>

              <div className="card">
                <div className="cardHead" style={{ marginBottom: 6 }}>
                  <h2 style={{ margin: 0 }}>Pillars (Article I powers)</h2>
                  <button
                    className="btn secondary"
                    onClick={() =>
                      setScaleMode((m) => (m === "letters" ? "traffic" : "letters"))
                    }
                  >
                    Toggle scale
                  </button>
                </div>
                <div className="muted small">
                  Each pillar includes a plain-language indicator and an evidence list.
                </div>

                <div className="pillars">
                  {PILLARS.map((p) => {
                    const data = selected.pillars?.[p.key] || {
                      status: "mid",
                      indicator: "No qualifying action recorded (yet).",
                      evidence: [
                        ev(
                          "—",
                          "No qualifying, verifiable action recorded in this period",
                          lastUpdated,
                          "Scorecard note"
                        ),
                      ],
                    };

                    return (
                      <details
                        key={p.key}
                        className="pillDetail"
                        open={p.key === "purse" || p.key === "oversight"}
                      >
                        <summary className="summary">
                          <span>{p.label}</span>
                          <span className={`chip ${data.status}`}>{data.status.toUpperCase()}</span>
                        </summary>
                        <div className="muted small" style={{ marginTop: 8 }}>
                          {data.indicator}
                        </div>

                        <div className="evidence">
                          {(data.evidence || []).map((e, idx) => (
                            <div className="ev" key={idx}>
                              <div className="evTop">
                                <span className="tag">{e.type}</span>
                                <span className="muted">
                                  {e.date} • {e.sourceLabel}
                                </span>
                              </div>
                              <div style={{ marginTop: 6 }}>
                                {e.url ? (
                                  <a href={e.url} target="_blank" rel="noreferrer">
                                    <strong>{e.title}</strong>
                                  </a>
                                ) : (
                                  <strong>{e.title}</strong>
                                )}
                              </div>
                            </div>
                          ))}
                        </div>
                      </details>
                    );
                  })}
                </div>
              </div>
            </div>
          </section>
        )}

        {view === "detail" && !selected && (
          <section className="card">
            <h2>Member not found</h2>
            <p className="muted">Return to the scorecard and select a member.</p>
            <button className="btn secondary" onClick={() => (window.location.hash = "")}>
              ← Back to scorecard
            </button>
          </section>
        )}

        {view === "method" && (
          <section className="card">
            <h2>Methodology (plain-spoken)</h2>
            <p className="muted">
              This scorecard is built to be easy to understand, hard to dispute, and difficult
              to ignore. We score only actions that are public, binary, and verifiable.
            </p>

            <h3>Principles we track</h3>
            <ul className="muted">
              <li>
                Focus on defending Congress’s Article I authority (aligned with the We the
                People Playbook principles, plus key additions).
              </li>
              <li>
                Pillars include: power of the purse, trade authority, emergency powers, war
                powers, domestic troop deployment, election authority, oversight/subpoena
                authority, and related Article I powers as needed.
              </li>
            </ul>

            <h3>What counts as evidence</h3>
            <ul className="muted">
              <li>Floor votes on relevant bills</li>
              <li>Co-sponsorship of specific bills or resolutions</li>
              <li>Signed letters</li>
              <li>Formal statements entered into the Congressional Record</li>
              <li>Optional (phase-in): additional public statements, once reliably captured</li>
            </ul>

            <h3>How grades work</h3>
            <p className="muted">
              Grades summarize how consistently a member takes defensible actions across
              pillars. The emphasis is deterrence and accountability: raising the reputational
              cost of institutional abdication while elevating positive examples of
              constitutional defense.
            </p>
          </section>
        )}

        {view === "about" && (
          <section className="card">
            <h2>About</h2>
            <p className="muted">
              Issue One, in collaboration with The Council for American Democracy (TCAD),
              created this scorecard as a public, pressure-focused accountability tool.
            </p>
            <ul className="muted">
              <li>Primary audience: Members of Congress and senior staff</li>
              <li>Also for: journalists, academics, advocates, and voters</li>
              <li>Initial scope: Senate + priority House races (expand later as needed)</li>
            </ul>
          </section>
        )}
      </main>

      <div id="toast" className="toast" />
    </div>
  );
}

const css = `
  :root{
    --bg:#0b0f19;
    --panel:#111827;
    --panel2:#0f172a;
    --text:#e5e7eb;
    --muted:#9ca3af;
    --line:#243244;
    --good:#22c55e;
    --mid:#f59e0b;
    --bad:#ef4444;
    --link:#93c5fd;
    --shadow: 0 10px 30px rgba(0,0,0,.35);
    --radius: 16px;
    --max: 1150px;
    --mono: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;
    --sans: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Apple Color Emoji","Segoe UI Emoji";
  }
  *{ box-sizing:border-box; }
  body{ margin:0; font-family: var(--sans); background: var(--bg); color: var(--text); }

  .page{
    min-height: 100vh;
    background:
      radial-gradient(1000px 700px at 20% -20%, rgba(59,130,246,.25), transparent 55%),
      radial-gradient(900px 600px at 120% 10%, rgba(239,68,68,.18), transparent 55%),
      var(--bg);
  }

  a{ color: var(--link); text-decoration:none; }
  a:hover{ text-decoration:underline; }

  .header{
    position: sticky;
    top: 0;
    z-index: 10;
    background: rgba(11,15,25,.75);
    backdrop-filter: blur(10px);
    border-bottom: 1px solid rgba(36,50,68,.65);
  }

  .wrap{ max-width: var(--max); margin: 0 auto; padding: 18px; }
  .main{ padding-top: 22px; padding-bottom: 42px; }

  .topbar{ display:flex; align-items:center; justify-content:space-between; gap:12px; }
  .brand{ display:flex; align-items:center; gap:10px; font-weight:700; letter-spacing:.2px; cursor:pointer; }
  .dot{ width:12px; height:12px; border-radius:999px; background: linear-gradient(135deg, #60a5fa, #34d399);
        box-shadow: 0 0 0 6px rgba(96,165,250,.10); }
  .nav{ display:flex; gap:10px; flex-wrap:wrap; }
  .navbtn{ padding:8px 10px; border-radius:999px; border:1px solid rgba(36,50,68,.8); background: rgba(17,24,39,.45);
           color: var(--text); font-size:13px; cursor:pointer; }
  .navbtn.active{ border-color: rgba(147,197,253,.85); box-shadow: 0 0 0 4px rgba(147,197,253,.12); }

  .hero{
    background: linear-gradient(180deg, rgba(17,24,39,.72), rgba(15,23,42,.55));
    border:1px solid rgba(36,50,68,.8);
    border-radius: var(--radius);
    box-shadow: var(--shadow);
    padding: 20px;
  }
  .hero h1{ margin:0 0 8px; font-size: 28px; }
  .hero p{ margin:0 0 12px; color: var(--muted); max-width: 75ch; }

  .meta{ display:flex; gap:12px; flex-wrap:wrap; align-items:center; color: var(--muted); font-size:13px; }
  .pill{ padding:6px 10px; border-radius:999px; background: rgba(31,41,55,.55); border:1px solid rgba(36,50,68,.8); }

  .controls{
    margin-top: 14px;
    display:grid;
    grid-template-columns: 1.2fr .8fr .8fr .8fr .8fr;
    gap:10px;
  }
  @media (max-width: 900px){ .controls{ grid-template-columns: 1fr 1fr; } }

  .control{
    background: rgba(17,24,39,.55);
    border:1px solid rgba(36,50,68,.8);
    border-radius: 12px;
    padding:10px;
    display:flex;
    flex-direction:column;
    gap:6px;
  }
  .control label{ font-size:12px; color: var(--muted); }
  .control input, .control select{ width:100%; background: transparent; border:0; outline:none; color: var(--text); font-size:14px; }
  .control select option{ background: var(--panel); }

  .row{ display:flex; justify-content:space-between; align-items:center; gap:12px; margin-top: 12px; flex-wrap:wrap; }
  .rowBtns{ display:flex; gap:10px; flex-wrap:wrap; }

  .btn{ background: rgba(59,130,246,.15); border:1px solid rgba(59,130,246,.45); color: var(--text);
        padding:10px 12px; border-radius: 12px; cursor:pointer; font-weight:600; font-size: 14px; }
  .btn.secondary{ background: rgba(31,41,55,.55); border-color: rgba(36,50,68,.85); }
  .btn:active{ transform: translateY(1px); }

  .panel{
    margin-top: 14px;
    background: rgba(17,24,39,.60);
    border:1px solid rgba(36,50,68,.8);
    border-radius: var(--radius);
    box-shadow: var(--shadow);
    overflow:hidden;
  }

  .tableWrap{ overflow:auto; }
  table{ width:100%; border-collapse: collapse; }
  th, td{ padding: 12px; border-bottom: 1px solid rgba(36,50,68,.7); text-align:left; vertical-align: middle; font-size:14px; }
  th{ color: var(--muted); font-size: 12px; text-transform: uppercase; letter-spacing: .08em; background: rgba(15,23,42,.50); }
  tr:hover td{ background: rgba(15,23,42,.45); }
  .clickable{ cursor:pointer; }

  .grade{ display:inline-flex; align-items:center; gap:8px; padding:6px 10px; border-radius:999px;
          background: rgba(31,41,55,.55); border:1px solid rgba(36,50,68,.85); font-weight: 800; }
  .mono{ font-family: var(--mono); }
  .dotg{ width:10px; height:10px; border-radius:999px; }
  .gA{ background: var(--good); }
  .gC{ background: var(--mid); }
  .gF{ background: var(--bad); }

  .memberCell{ display:flex; align-items:center; gap:10px; }
  .avatar{ width:34px; height:34px; border-radius:999px; object-fit:cover; border:1px solid rgba(36,50,68,.8); box-shadow: 0 8px 18px rgba(0,0,0,.25); background: rgba(17,24,39,.6); }
  .avatar.lg{ width:54px; height:54px; }
  .nameBlock{ display:flex; align-items:center; gap:12px; }

  .chips{ display:flex; gap:6px; flex-wrap:wrap; }
  .chip{ font-size: 12px; padding: 6px 8px; border-radius: 999px; background: rgba(31,41,55,.55);
         border: 1px solid rgba(36,50,68,.8); color: var(--text); white-space:nowrap; }
  .chip.good{ border-color: rgba(34,197,94,.55); }
  .chip.mid{ border-color: rgba(245,158,11,.55); }
  .chip.bad{ border-color: rgba(239,68,68,.55); }

  .tag{ font-size:12px; padding:4px 8px; border-radius:999px; background: rgba(31,41,55,.55);
        border:1px solid rgba(36,50,68,.75); color: var(--muted); font-family: var(--mono); margin-left: 8px; }

  .card{
    background: rgba(17,24,39,.60);
    border:1px solid rgba(36,50,68,.8);
    border-radius: var(--radius);
    box-shadow: var(--shadow);
    padding: 16px;
  }

  .detailGrid{ display:grid; grid-template-columns: 1fr .9fr; gap: 14px; margin-top: 14px; }
  @media (max-width: 900px){ .detailGrid{ grid-template-columns: 1fr; } }

  .cardHead{ display:flex; align-items:center; justify-content:space-between; gap: 12px; }

  .muted{ color: var(--muted); }
  .small{ font-size: 13px; }

  .kv{ display:grid; grid-template-columns: 140px 1fr; gap: 8px 12px; margin-top: 10px; font-size: 14px; }
  .kv div:nth-child(odd){ color: var(--muted); }

  .pillars{ margin-top: 10px; display:flex; flex-direction:column; gap: 10px; }
  .pillDetail{ border:1px solid rgba(36,50,68,.8); border-radius: 14px; background: rgba(15,23,42,.42); padding: 10px 12px; }
  .summary{ cursor:pointer; font-weight:700; display:flex; align-items:center; justify-content:space-between; gap:12px; }

  .evidence{ margin-top: 10px; border-top: 1px solid rgba(36,50,68,.7); padding-top: 10px; display:flex; flex-direction:column; gap: 8px; }
  .ev{ padding:10px 12px; border-radius: 12px; background: rgba(17,24,39,.55); border:1px solid rgba(36,50,68,.7); }
  .evTop{ display:flex; justify-content:space-between; gap:10px; flex-wrap:wrap; font-size: 13px; }

  .toast{ position:fixed; bottom:16px; left:50%; transform:translateX(-50%);
          background: rgba(17,24,39,.92); border:1px solid rgba(36,50,68,.9); color: var(--text);
          padding:10px 12px; border-radius: 12px; box-shadow: var(--shadow); display:none; z-index: 99; }
`;
