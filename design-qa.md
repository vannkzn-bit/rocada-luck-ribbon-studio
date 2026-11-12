# Design QA — reference composition v2

Status: passed for design sandbox, 2026-11-12.

Compared the actual Safari 800 × 800 preview against the cropped supplied screenshot in qa/comparison.png. Desktop columns, tape center, prize spacing, right logo, QR, caption and button align with the reference. Removed stray neighboring tape fragments at the top and bottom after the first comparison. Desktop start → spin → win → promo → restart completed in Safari. Mobile 390 × 780 preview inspected: all content fits, tape horizontal at top, no clipped controls; spin launch verified. Old save is retained separately, version 1 imports are supported.

Automated checks: 308 stopping positions, import validation, zero-valued settings, legacy version migration, all six bundled data images, JavaScript syntax. No dependencies or external image requests.

Known intentional differences: real demo QR points to this sandbox; background and gift are reconstructed image assets; logos are low-resolution screenshot extracts with faint backgrounds. Original brand graphics can replace these via the editor. Mobile arrangement is an adaptation because the reference only shows desktop. This is not the Mindbox runtime or a reverse-importable campaign.

Screenshots remain local in qa/ to avoid publishing browser chrome or the original desktop capture.

Final user adjustment verified in Safari: separate logo, QR and caption hidden; background, tape and arrows retained. Button center is y=400 on 800×800 canvas, aligned with both pointer centers. Final screenshot: qa/final-preview.png. This deliberate simplification supersedes the initial screenshot composition.
