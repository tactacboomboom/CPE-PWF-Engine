🟧 𝕍 — Validateur de contrat (gate)

**Type** : 🟧 Filtre validation

**[IDENTITÉ]** 𝕍 : 𝕮₁ → (PASS/FAIL, diagnostic, actions)  
**[FINALITÉ]** Empêcher l’exécution sur contrat flou / toxique / non testable  
**[ENTRÉES]** 𝕮₁  
**[SORTIES]**

1. PASS → autorise μ₁
2. FAIL → renvoie vers correction de 𝕮₁ (ou κ₀)

**[INVARIANTS]**

1. Diagnostic **actionnable** (quoi changer, où, pourquoi)
2. Critères stables (mêmes règles à chaque sprint)

**[RÈGLES D’ACTIVATION]**

1. Obligatoire **avant** μ₁
2. Ré-exécuter si 𝕮₁ change

**[ANTI-PATHOLOGIES]**

1. ❌ validation “rhétorique” (opacité)
2. ❌ FAIL sans action
3. ❌ PASS permissif (laisse passer du flou)

**[POSITION DANS LA CHAÎNE]** entre 𝕮₁ et μ₁  
**[POSITION (x,y)]** (x=12, y=0)
