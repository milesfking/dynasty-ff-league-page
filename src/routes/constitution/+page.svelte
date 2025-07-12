<script>
    import { dues } from '$lib/utils/helper';
    let one, oneOne, oneOneOne, oneTwo, oneThree;
    let two, twoOne, twoTwo, twoThree;
    let three, threeOne;
    let four, fourOne, fourTwo;
    let five, fiveOne;
    let six, sixOne, sixTwo, sixThree;
    let seven, sevenOne, sevenTwo, sevenThree;

    const goToSection = (section) => {
        const top = section.getBoundingClientRect().top + window.pageYOffset;
        window.scrollTo({left: 0, top, behavior: 'smooth'});
    }
</script>

<style>
    .constitution {
        position: relative;
        z-index: 1;
        width: 92%;
        max-width: 800px;
        margin: 8em auto 10em;
    }

    h1 {
        font-size: 2em;
        line-height: 1.2em;
        text-align: center;
        margin: 2em 0 1.5em;
    }

    h2 {
        font-size: 1.5em;
        line-height: 1.2em;
    }

    h3 {
        text-decoration: underline;
        font-size: 1.3em;
        line-height: 1.2em;
    }

    h4 {
        text-decoration: underline;
        margin-left: 2em;
        font-size: 1.2em;
        line-height: 1.2em;
    }

    h5 {
        margin-left: 6em;
        font-size: 0.8em;
        line-height: 1.1em;
    }

    .subBlock {
        margin-left: 2.4em;
    }

    .sectionHeading {
        margin: 4em 0 1.5em;
    }

    .subSectionHeading {
        margin: 1.5em 0 1.5em;
    }

    .underscore {
        text-decoration: underline;
    }

    .right {
        text-align: right;
    }

    .positionMaximums td {
        min-width: 3em;
    }

    .noUnderscore {
        text-decoration: none;
    }

    .clickable {
        cursor: pointer;
    }

    .clickable:hover {
        color: #00316b;
    }

    p {
        color: #777;
    }
</style>

<div class="constitution">
    <h1 class="noUnderscore">LEAGUE CONSTITUTION</h1>
    
    <h2 class="noUnderscore">TABLE OF CONTENTS</h2>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(one)}>Section 1: Roster</h3>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(oneOne)}>1.1 Roster Structure</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(oneTwo)}>1.2 Starting Lineup</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(oneThree)}>1.3 Taxi Squad</h4>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(two)}>Section 2: Trading</h3>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(twoOne)}>2.1 Trade Vetoes</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(twoTwo)}>2.2 Trade Deadline</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(twoThree)}>2.3 Draft Pick Trading</h4>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(three)}>Section 3: Waiver Wire</h3>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(threeOne)}>3.1 FAAB System</h4>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(four)}>Section 4: Rookie Draft</h3>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(fourOne)}>4.1 Draft Format</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(fourTwo)}>4.2 Draft Order</h4>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(five)}>Section 5: Playoffs</h3>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(fiveOne)}>5.1 Playoff Format</h4>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(six)}>Section 6: Scoring</h3>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sixOne)}>6.1 Scoring System</h4>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(seven)}>Section 7: League Finances</h3>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sevenOne)}>7.1 Buy-In</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sevenTwo)}>7.2 Payout</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sevenThree)}>7.3 Leaving the League</h4>
    
    
    <hr />
    
    <h2 class="sectionHeading" bind:this={one}>Section 1: Roster</h2>
    
    <h3 class="subSectionHeading" bind:this={oneOne}>1.1 Roster Structure</h3>
    
    <p>Rosters will be composed of 23 active roster spots (12 starters and 11 bench spots), 2 IR spots, and 4 Taxi squad spots.</p>
    
    <h3 class="subSectionHeading" bind:this={oneTwo}>1.2 Starting Lineup</h3>
    
    <p class="underscore">Starters</p>
    <ul>
        <li>QB</li>
        <li>RB</li>
        <li>RB</li>
        <li>WR</li>
        <li>WR</li>
        <li>WR</li>
        <li>TE</li>
        <li>Flex (RB/WR/TE)</li>
        <li>Fles (RB/WR/TE)</li>
        <li>Superflex (QB/RB/WR/TE)</li>
        <li>K</li>
        <li>DST</li>
    </ul>
    
    <h3 class="subSectionHeading" bind:this={oneThree}>1.3 Taxi Squad</h3>
    
    <p>The Taxi Squad is a Sleeper default setting that gives members incentive to hold on to rookie bums who won't play for a while. There are 4 taxi squad spots. *Players can only be added to the taxi squad prior to the beginning of their rookie season, but once on the squad, they can stay there through their second year.* Players can be activated to the main roster at any time, but, once activated, cannot be put on the taxi squad again.</p>
    
    <h2 class="sectionHeading" bind:this={two}>Section 2: Trading</h2>
    
    <h3 class="subSectionHeading" bind:this={twoOne}>2.1 Trade Vetoes</h3>
    <p>Commish has veto power. Like in the redraft league, trades will only be vetoed if they are clear collusion and/or significantly impact the competitive balance of the league. A simple fleece is not enough for a trade to be vetoed. The league can overrule a veto with a two-thirds vote.</p>
    
    <h3 class="subSectionHeading" bind:this={twoTwo}>2.2 Trade Deadline</h3>
    <p>The trade deadline is Week 13 (two weeks before the playoffs start) and the trade window will re-open during the offseason.</p>
    
    <h3 class="subSectionHeading" bind:this={twoThree}>2.3 Draft Pick Trading</h3>
    <p>Draft picks are eligible to be traded up to two years in advance. For instance, this year you will be able to trade picks in the 2025 and 2026 rookie drafts. You must pay the buy-in for any year in which you are trading or acquiriing a pick. For example, if you have bought in for 2024 but want to trade for (or trade away) a 2025 pick, you need to commit to paying 2025 buy-in too. We are all friends so you won't be required to pay for future years immediately, but you will be held to this.</p>
    
    <h2 class="sectionHeading" bind:this={three}>Section 3: Waiver Wire</h2>
    
    <h3 class="subSectionHeading" bind:this={threeOne}>3.1 FAAB System</h3>
    <p>The league waivers will be FAAB. Each player will be allocated $200 to spend on waiver wire pickups throughout the season. This amount will reset when waivers re-open for the first timeafter the Super Bowl.</p>
    
    <p>Players on waivers will be locked upon the start of their week's game. During the season, waivers will clear Wednesday morning. If a player is dropped to the waiver wire, they will be ineligible to be picked up for two days, even if waivers have cleared for the week. In the offseason, waivers will be processed once every week on Wednesdays.</p>
    
    <h2 class="sectionHeading" bind:this={four}>Section 4: Rookie Draft</h2>
    
    <h3 class="subSectionHeading" bind:this={fourOne}>4.1 Draft Format</h3>
    <p>The draft will be 4 rounds, and each team will have a pick in each round. Unlike the startup draft, the rookie drafts will be linear, meaning if you suck ass you will have the 1.1 (round 1 pick 1), 2.1, 3.1, and 4.1.</p>
    
    <h3 class="subSectionHeading" bind:this={fourTwo}>4.2 Draft Order</h3>
    
    <p class="underscore">Non-Playoff Teams</p>
    <p>Draft order will be determined by Maximum Points For, or how many points your team would have scored if you set your lineup optimally all season. The lowest Max Points For for a non-playoff team will be awarded the first pick, and the highest for a non-playoff team will be awarded the sixth.</p>
    
    <p class="underscore">Playoff Teams</p>
    <p>As in the NFL, the remaining order will be determined by playoff performance. The league winner will receive the #12, second place will receive #11, third place will receive #10, and fourth place will receive #9. To incentivize provide incentive in the 5th/6th place game, the winner of that game will receive the #7 pick and the loser will receive the #8.</p>
    
    <h2 class="sectionHeading" bind:this={five}>Section 5: Playoffs</h2>
    
    <h3 class="subSectionHeading" bind:this={fiveOne}>5.1 Playoff Format</h3>
    <p>The playoff format will be the same as the redraft league—6 teams, with the top two teams receiving a bye. The playoffs will commence Week 15 and end Week 17. Each round will be one week. As there are no divisions, seeding will be based on record.</p>
    
    <h2 class="sectionHeading" bind:this={six}>Section 6: Scoring</h2>
    
    <h3 class="subSectionHeading" bind:this={sixOne}>6.1 Scoring System</h3>
    <p>Standard Sleeper scoring unless otherwise noted. Exceptions follow.</p>
    
    <p class="underscore">Half-PPR, Half-PPFD</p>
    <p>We will continue a half-PPR (half-point-per-reception), half-PPFD (half-point-per-first-down) league.</p>
    
    <p class="underscore">Tight End Premium</p>
    <p>Tight ends receive an additional half-point boost per reception, so tight ends get 1 full PPR.</p>

    <h2 class="sectionHeading" bind:this={seven}>Section 7: League Finances</h2>
    
    <h3 class="subSectionHeading" bind:this={sevenOne}>7.1 Buy-In</h3>
    <p>The buy-in is $30, to be paid in full at the start of the season.</p>
    
    <h3 class="subSectionHeading" bind:this={sevenTwo}>7.2 Season Payout</h3>
    <p>Of the $30 buy-in, $25 will be allocated to the current season, for a total pot of $300. Third place will receive $25, second place will receive $50, and first place will receive the remaining $225.</p>
    
    <h3 class="subSectionHeading" bind:this={sevenTwo}>7.3 Empire Payout</h3>
    <p>The remaining $5 per person (totaling $60 per season) will be allocated to the empire pot. If someone triggers the empire clause, they will win the entire empire pot (minimum $120) in addition to first place payout.</p>

    <h3 class="subSectionHeading" bind:this={sevenThree}>7.4 Leaving the League</h3>
    <p>Not allowed. Jk, if you no longer want to be involved that's fine, but it is your responsibility to find a replacement owner. In a lot of cases, it is hard to find someone to take over a shitty team, so you might need to pay the entry fee for the following year to make a successful transition. Just be aware of that. Remember that the league will also reset, at which point you will be able to leave without needing to transition to a new owner.</p>

</div>