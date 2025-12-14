# 🛡️ SESSION SAFETY & QUALITY PROTOCOL

## Critical Rules for This Build Session

### 1. QUALITY MANDATES (Non-Negotiable)

**Every design package MUST:**
- Use UNIQUE color palettes (no copy-paste between sites)
- Have COMPLETE CSS tokens (70+ variables minimum)
- Include DETAILED v0 prompts (100+ lines each with exact specs)
- Specify EXACT hex values, font sizes, spacing
- List EXPLICIT anti-patterns in every prompt
- Feel like a premium agency delivered it

**Every v0 prompt MUST include:**
- Complete color palette with all shades
- Typography scale (every size used)
- Spacing system (8px grid values)
- Component-specific specs (dimensions, animations, states)
- MUST INCLUDE section (required elements)
- MUST NOT INCLUDE section (anti-patterns)
- Exact copy/text to use
- Responsive behavior specifications
- Animation/interaction details

### 2. DATA SAFETY PROTOCOL

**Save checkpoints after:**
- [ ] Each site's CSS tokens complete
- [ ] Each site's Tailwind config complete
- [ ] Each site's v0 prompts complete
- [ ] Each site's CLAUDE.md complete
- [ ] Each site's full package zipped

**Checkpoint format:**
```
/home/claude/checkpoints/
├── checkpoint-1-wealthfromai-tokens.md
├── checkpoint-2-wealthfromai-prompts.md
├── checkpoint-3-wealthfromai-complete.zip
└── session-progress.json
```

**Progress tracker:**
```json
{
  "session_start": "2025-12-13T23:00:00Z",
  "sites_completed": [],
  "sites_in_progress": [],
  "last_checkpoint": "",
  "total_files_created": 0
}
```

### 3. TOKEN LIMIT AWARENESS

**Warning signs to watch:**
- Response getting truncated
- File creation incomplete
- Context becoming confused

**Mitigation actions:**
- Complete current site fully
- Save all work to outputs
- Create continuation prompt
- Document exactly where we stopped

**Continuation prompt template:**
```markdown
## CONTINUATION FROM PREVIOUS SESSION

### What Was Completed:
[List completed sites and files]

### What's In Progress:
[Current site and status]

### What Remains:
[List remaining sites]

### Resume Instructions:
[Specific next action]

### Critical Context:
- All design packages at: /home/claude/[SiteName]-DesignPackage/
- Battle plan at: /home/claude/7-SITE-BATTLE-PLAN.md
- Progress tracker at: /home/claude/checkpoints/session-progress.json
```

### 4. FILE SIZE MANAGEMENT

**For large files (>300 lines):**
- Create in chunks
- Save after each chunk
- Verify file integrity
- Never lose work to truncation

**Chunk pattern:**
```
# Create file header
# Save checkpoint
# Add section 1 (colors)
# Save checkpoint  
# Add section 2 (typography)
# Save checkpoint
# Continue...
```

### 5. AFFILIATE INTEGRATION REQUIREMENTS

**For each review site (4 sites):**
- Amazon PAAPI integration template
- Product comparison table component
- Single product review block
- Rating system component
- Pros/cons layout
- "Best for" badges
- Affiliate disclosure placement
- Price display patterns
- CTA button styles

**Affiliate disclosure rules:**
- FTC-compliant disclosure
- Above-the-fold placement
- Clear, readable text
- Consistent across site

### 6. NO SHORTCUTS LIST

**We will NOT:**
- ❌ Use generic color palettes
- ❌ Copy tokens between sites
- ❌ Use vague v0 prompts
- ❌ Skip anti-pattern lists
- ❌ Use placeholder text
- ❌ Rush any component
- ❌ Skip responsive specs
- ❌ Ignore animation details
- ❌ Use default fonts
- ❌ Create "good enough" work

**We WILL:**
- ✅ Research each niche thoroughly
- ✅ Create unique identities
- ✅ Specify exact values everywhere
- ✅ Test against anti-patterns
- ✅ Save progress constantly
- ✅ Document everything
- ✅ Create masterpiece quality
- ✅ Think like a $50K agency

### 7. SKILLS TO LOAD FOR EACH SITE

Before starting each site:
```
1. /mnt/skills/user/wordpress-empire-system/SKILL.md
2. /mnt/skills/user/wordpress-blocks/SKILL.md
3. /mnt/skills/user/n8n-master-architect/SKILL.md
4. /mnt/skills/examples/frontend-design/SKILL.md (if exists)
5. /home/claude/visual-to-code-pipeline/SKILL.md
6. /home/claude/v0-automation/SKILL.md
7. NEW: /home/claude/affiliate-content-system/SKILL.md
8. NEW: /home/claude/tech-review-templates/SKILL.md
```

### 8. EXECUTION ORDER (Optimized)

**Group by theme type for efficiency:**

**Round 1: Dark Premium Sites**
1. wealthfromai.com (Navy + Gold, Premium dark)
2. aiinactionhub.com (Neon cyan, Futuristic dark)

**Round 2: Light Editorial Sites**  
3. clearainews.com (Editorial blue, Clean white)
4. aidiscoverydigest.com (Indigo, Curated clean)

**Round 3: Tech Review Sites**
5. smarthomegearreviews.com (Trust blue)
6. wearablegearreviews.com (Health teal)
7. pulsegearreviews.com (Energy red)

### 9. DELIVERABLE CHECKLIST PER SITE

```
□ CLAUDE.md (complete project config)
□ design-reference/tokens/variables.css (70+ vars)
□ design-reference/tokens/tailwind.config.js (complete theme)
□ design-reference/v0-prompts/hero.md (100+ lines)
□ design-reference/v0-prompts/navigation.md (80+ lines)
□ design-reference/v0-prompts/cards.md (100+ lines)
□ design-reference/v0-prompts/newsletter.md (80+ lines)
□ design-reference/v0-prompts/footer.md (80+ lines)
□ affiliate-templates/ (for review sites only)
□ docs/brand-guide.md
□ Checkpoint saved
□ Zipped and copied to outputs
```

### 10. QUALITY GATES

Before marking any site complete:

**Design Token Check:**
- [ ] All colors have light/dark variants
- [ ] Typography has complete scale (xs through 5xl)
- [ ] Spacing uses consistent 8px grid
- [ ] Shadows defined for all elevation levels
- [ ] Border radius has complete scale
- [ ] Animation values specified

**v0 Prompt Check:**
- [ ] Exact hex codes (not "blue" or "primary")
- [ ] Exact font names from Google Fonts
- [ ] Exact pixel/rem values
- [ ] States defined (hover, focus, active)
- [ ] Responsive breakpoints specified
- [ ] Anti-patterns listed (minimum 5)
- [ ] Exact copy text provided

**Brand Check:**
- [ ] Unique from all other sites
- [ ] Matches niche expectations
- [ ] Professional agency quality
- [ ] Would win design awards
- [ ] Feels human-crafted

---

## Session Commands

**Save checkpoint:**
```bash
mkdir -p /home/claude/checkpoints
echo '{"status": "checkpoint", "site": "[NAME]", "time": "'$(date -Iseconds)'"}' >> /home/claude/checkpoints/session-progress.json
```

**Create continuation prompt:**
```bash
cat > /home/claude/checkpoints/CONTINUE-FROM-HERE.md << 'EOF'
[Continuation details]
EOF
```

**Emergency save all:**
```bash
cd /home/claude && zip -r emergency-backup-$(date +%Y%m%d-%H%M%S).zip *-DesignPackage/ checkpoints/ && cp *.zip /mnt/user-data/outputs/
```
