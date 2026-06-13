---
name: gaokao-application-advisor
description: Use when Codex helps with China Gaokao college application planning,志愿填报,院校专业组/专业选择,冲稳保梯度,位次法分析,招生章程核验,高考分数和省排名匹配,就业薪酬前景,行业发展趋势,职业路径分析, or comparing Chinese universities/majors for undergraduate admission. Always use current official provincial admissions rules, enrollment plans, school admissions charters, current labor-market sources, and the user's province/year/score/rank/subjects/preferences before giving recommendations.
---

# Gaokao Application Advisor

Use this skill to help a user build a careful, evidence-based Gaokao application plan. Treat the work as decision support, not a guarantee of admission.

## First Clarify Inputs

Before recommending schools or majors, collect the minimum viable profile:

- Province and application year
- Exam track or selected subjects
- Score, provincial rank/位次, and batch/control line
- Preferred majors, disliked majors, city/region constraints, tuition constraints
- Risk appetite: aggressive, balanced, or conservative
- Whether the user prioritizes school reputation, major strength, city, employment, postgraduate options, or admission certainty
- Career orientation: high salary, stable employment, public-sector paths, graduate study, technical depth, entrepreneurship, family location, or work-life balance
- Special constraints: physical exam limits, color blindness/weakness, language restrictions, single-subject requirements, gender restrictions if legally listed in official plan, household registration or ethnic policy, Chinese-foreign cooperative programs, public/private preference

If the user lacks rank, explain that rank/位次 is usually more reliable than raw score for cross-year matching and ask for it. If the user only has score, proceed with provisional analysis and label it as provisional.

## Source Requirements

For current-year advice, verify facts with current sources. Prefer:

1. Provincial education examination authority / 招生考试院
2. Official current-year enrollment plan / 招生计划
3. University undergraduate admissions website / 本科招生网
4. Current-year admissions charter / 招生章程
5. Ministry of Education or Sunshine Gaokao where relevant
6. Current labor-market and salary sources: official graduate employment quality reports, university就业质量报告, Ministry of Human Resources and Social Security information, National Bureau of Statistics data, industry association reports, reputable recruitment-platform salary reports, and recent employer demand reports

Use third-party datasets only as auxiliary references, never as the sole basis for final advice. When current-year data is unavailable, state the limitation and use the latest available official data plus clear uncertainty labels.

Read `references/checklist.md` when doing a full志愿方案 or when the user asks for学校/专业推荐. Read `references/career-market.md` when comparing majors, salary prospects, industry development, or就业质量.

## Workflow

1. Build the user profile and confirm missing high-impact fields.
2. Identify the province's admission model: traditional batch, parallel志愿,院校专业组,专业+院校, or other local variant.
3. Establish historical matching by rank, not just score. Compare at least 2-3 recent years when data is available.
4. Segment candidate choices into risk bands:
   - 冲: historical admission rank usually better than user's rank; use sparingly.
   - 稳: historical rank roughly near user's rank with reasonable margin.
   - 保: historical rank safely behind user's rank.
   - 兜底: strong likelihood under normal conditions; include to avoid滑档/退档 risk.
5. Check major-level constraints, not just school-level minimums.
6. Check admissions charter rules: major allocation, grade difference, single-subject limits, physical exam requirements, transfer policy, and whether调剂 is available.
7. Analyze each candidate major against the current five-year employment market:
   - recent salary trend and realistic entry salary band
   - employment stability and demand concentration by city/industry
   - career ladder after 3-5 years
   - postgraduate,考公,考编,资格证, and转码/转行 paths
   - automation/AI substitution risk and cyclicality risk
8. For each recommended institution, recommend concrete majors or院校专业组 combinations, not just the school name.
9. Produce a ranked recommendation table and risk notes.
10. End with a verification list of official documents the user should review before submission.

## Recommendation Format

For full plans, provide a table with:

- Band: 冲 / 稳 / 保 / 兜底
- Institution
- Major or院校专业组
- City/province
- Evidence: historical最低位次/投档位次, year, and source
- Recommended majors in that institution, ordered by fit
- Employment view: salary outlook, industry trend, 3-5 year path, and main downside
- Fit reason
- Main risk
- Action: keep, verify, replace, or only consider if user accepts tradeoff

Keep the tone practical and non-alarmist. Do not imply certainty. Use phrases like "风险偏高", "相对稳妥", "需要核验招生章程", and "以当年官方投档和招生计划为准".

## Decision Guardrails

Never recommend solely from brand ranking. A prestigious university with an unsuitable major, restrictive transfer policy, or high退档 risk may be a poor choice.

Never recommend a school without naming the specific major(s) or院校专业组 worth filling. If the school is only attractive for a few majors, say so and do not imply that all majors at the school are equally good.

Never use salary rankings mechanically. Explain whether a high salary reflects a small elite sample, a first-tier-city concentration, graduate-degree dependence, industry boom-cycle effects, or high attrition.

Never ignore专业限制. For medical, military, police, navigation, aviation, normal-university公费师范, art/sport, Chinese-foreign cooperative, and special-plan admissions, explicitly check extra rules.

When the user asks for "最好的学校", translate that into a preference tradeoff: admission probability, major quality, city, future employment, graduate study, tuition, and family constraints.

If the request involves a province, year, policy, score line, enrollment plan,学校章程, salary, employment market, or industry trend that may have changed, browse or ask the user for official/current files before finalizing.
