```cpp
// profile.hpp — afuckingco's README
#pragma once

#include <array>
#include <string>
#include <string_view>
#include <vector>

namespace afuckingco {

inline constexpr std::string_view HANDLE    = "afuckingco";
inline constexpr std::string_view NAME      = "Afiq";
inline constexpr std::string_view TAGLINE   =
    "Security Research · Applied ML · Full-stack Systems. "
    "I turn chaotic signal into something structured, measurable, and useful.";

enum class Domain : std::uint8_t { Security, ML, Web, Embedded };

struct Contact  { std::string github, linkedin, email; };
struct Project  { std::string name, link, stack, blurb; };

class Developer {
public:
    Developer() : contact_{
        "https://github.com/afuckingco",
        "https://www.linkedin.com/in/afiq-andico",
        "anotherwaltzcompany@gmail.com",
    } {}

    [[nodiscard]] constexpr std::string_view handle()  const noexcept { return HANDLE;  }
    [[nodiscard]] constexpr std::string_view name()    const noexcept { return NAME;    }
    [[nodiscard]] constexpr std::string_view tagline() const noexcept { return TAGLINE; }
    [[nodiscard]] const Contact& contact() const noexcept { return contact_; }

    std::vector<std::string> focus = {
        "LSTM partial-reset dynamics",
        "security writeups & recon methodology",
        "PILGRIMS framework v17",
    };

private:
    Contact contact_;
};

inline const std::vector<Project> PROJECTS = {
    // ML
    {"lstm-partial-reset",  "https://github.com/afuckingco/lstm-partial-reset",   "Python",
     "LSTM time-series forecasting with partial-reset dynamics."},
    {"portfolio-showcase",  "https://github.com/afuckingco/portfolio-showcase",   "Multi",
     "15+ projects across ML, Security, Web, Embedded, GIS."},
    // Security
    {"security-writeups",   "https://github.com/afuckingco/security-writeups",    "—",
     "Authorized bug-bounty & security research writeups."},
    {"security-ops-suite",  "https://github.com/afuckingco/security-ops-suite",   "JavaScript",
     "CLI scanners, CI pipelines, log anonymizer, PILGRIMS framework."},
    {"code-audit-toolkit",  "https://github.com/afuckingco/code-audit-toolkit",   "AI",
     "Unified code-audit workflow across 6 AI endpoints."},
    {"pilgrims",            "https://github.com/afuckingco/pilgrims",             "Shell",
     "PILGRIMS v17.0 — 20-module security framework."},
    // Web
    {"secure-express-shop", "https://github.com/afuckingco/secure-express-shop",  "JavaScript",
     "Security-hardened Express e-commerce starter."},
    {"tokokita",            "https://github.com/afuckingco/tokokita",             "JavaScript",
     "Hardened Node.js shop: helmet, CSRF, rate-limit, atomic stock."},
    {"pahchinsan-studio",   "https://github.com/afuckingco/pahchinsan-studio",    "Astro",
     "Developer studio & portfolio site (Astro + Tailwind + daisyUI)."},
};

} // namespace afuckingco
```

<div align="center">

### `Developer me;` → **Afiq · afuckingco**

*"What I cannot create, I do not understand."* — R. Feynman

</div>

---

## ⚡ Quick Specs

| field | value |
|---|---|
| **repos** | 10 public |
| **domains** | `Security` · `ML` · `Web` · `Embedded` |
| **languages** | `Python` · `TypeScript` · `JavaScript` · `C` · `Shell` |
| **frameworks** | `Next.js` · `Express` · `Astro` · `Tailwind` · `PyTorch` · `XGBoost` |
| **open to** | security research · ML consulting · web projects |

---

## 🔧 Tech

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![Shell](https://img.shields.io/badge/Shell-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![Astro](https://img.shields.io/badge/Astro-FF5D01?style=flat-square&logo=astro&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

---

## 📂 Projects

**ML** — [lstm-partial-reset](https://github.com/afuckingco/lstm-partial-reset) · [portfolio-showcase](https://github.com/afuckingco/portfolio-showcase)

**Security** — [security-writeups](https://github.com/afuckingco/security-writeups) · [security-ops-suite](https://github.com/afuckingco/security-ops-suite) · [code-audit-toolkit](https://github.com/afuckingco/code-audit-toolkit) · [pilgrims](https://github.com/afuckingco/pilgrims)

**Web** — [secure-express-shop](https://github.com/afuckingco/secure-express-shop) · [tokokita](https://github.com/afuckingco/tokokita) · [pahchinsan-studio](https://github.com/afuckingco/pahchinsan-studio)

---

## 📊 Stats

<div align="center">
  <img height="155" src="https://github-readme-stats.vercel.app/api?username=afuckingco&show_icons=true&theme=github_dark&hide_border=true&count_private=true&include_all_commits=true" alt="GitHub Stats" />
  <img height="155" src="https://github-readme-stats.vercel.app/api/top-langs/?username=afuckingco&layout=compact&theme=github_dark&hide_border=true&langs_count=8" alt="Top Languages" />
</div>

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=afuckingco&theme=github_dark&hide_border=true" alt="GitHub Streak" />
</div>

---

## 🔭 Focus

- `in_progress` LSTM partial-reset forecasting
- `in_progress` security writeups & recon docs
- `in_progress` PILGRIMS v17

---

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-afuckingco-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/afuckingco)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Afiq%20Andico-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/afiq-andico)
[![Email](https://img.shields.io/badge/Email-anotherwaltzcompany%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:anotherwaltzcompany@gmail.com)

```cpp
// dS/dt ≥ 0    —    the second law holds for codebases too
// ΔE · Δt ≥ ℏ/2
```

</div>

```cpp
// EOF
```
