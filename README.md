- 👋 Hi, I’m Sayyed Saif (aka 0xsa1f)
- 👀 I’m interested in coding & hacking.
- 📫 Contact: 0xs41f@gmail.com

<!---
0xsa1f/0xsa1f is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
# 🌸 My recent AniList activity

<!-- ANILIST_ACTIVITY:start -->

<!-- ANILIST_ACTIVITY:end -->


name: AniList readme workflow
on:
    schedule:
        # Runs every hour
        - cron: "0 * * * *"
    workflow_dispatch:

jobs:
    update-readme-with-anilist:
        name: Update this repo's README with latest AniList activites
        runs-on: ubuntu-latest
        steps:
            - uses: actions/checkout@v2
            - name: AniList readme workflow
              uses: pxseu/anilist-readme@v1.2.1
              with:
                  user_id: 0xs41f
