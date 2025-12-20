```asm
; ==================================================
;  README.asm — Cz
; ==================================================
; Author   : Cz
; School   : EPITECH Nice
; Domain   : Development & Cybersecurity
; Status   : Student / Learner / Builder
; ==================================================

SECTION .boot
    MOV     USERNAME,    "Cz"
    MOV     ROLE,        "IT Student @ EPITECH Nice"
    MOV     MINDSET,     "Learn | Experiment | Code"
    MOV     CURIOSITY,   HIGH

    CALL    INIT_PROFILE

; --------------------------------------------------
SECTION .profile
INIT_PROFILE:
    PUSH    PASSION
    PUSH    DISCIPLINE
    PUSH    CURIOSITY

    MOV     PASSION,     DEV + CYBERSEC
    MOV     GOAL,        "Acquire skills & master new technologies"
    RET

; ==================================================
; TECH STACK
; ==================================================
SECTION .tech_stack
    ; Low-level & scripting
    DB  "C", 0
    DB  "Lua", 0
    DB  "Python", 0

    ; Web technologies
    DB  "JavaScript", 0
    DB  "TypeScript", 0
    DB  "HTML5", 0
    DB  "CSS3", 0
    DB  "TailwindCSS", 0

    ; Frameworks & runtimes
    DB  "Vue.js", 0
    DB  "React", 0
    DB  "Node.js", 0
    DB  "Django", 0
    DB  "PHP", 0

; ==================================================
; TOOLS & ENVIRONMENT
; ==================================================
SECTION .tools
    DB  "Git", 0
    DB  "npm", 0
    DB  "MySQL", 0
    DB  "phpMyAdmin", 0

; ==================================================
; OPERATING SYSTEMS
; ==================================================
SECTION .os
    DB  "Ubuntu", 0
    DB  "Windows", 0

; ==================================================
; INTEREST REGISTERS
; ==================================================
SECTION .interests
    MOV     R1, CYBERSECURITY     ; Attack & Defense
    MOV     R2, INFRASTRUCTURE    ; Systems & Networks
    MOV     R3, DEVELOPMENT       ; Software Engineering

; ==================================================
; GITHUB METRICS
; ==================================================
SECTION .metrics
    ; Runtime statistics fetched externally
    ; github-readme-stats.vercel.app
    MOV     GITHUB_USER, "Celz-Pch"

    CALL    FETCH_STATS
    CALL    FETCH_LANG_USAGE

; ==================================================
; END OF FILE
; ==================================================
HLT
```
