```asm
BITS 64
DEFAULT REL

SECTION .boot
    MOV USER,    "Cz"
    MOV ROLE,    "IT Student @ EPITECH Nice"
    MOV STACK,   DEV | CYBERSEC
    MOV PASSION, PHYSICS | MATHS

    CALL PROFILE
    CALL STATS
    HLT

SECTION .profile
PROFILE:
    MOV MINDSET, "Learn • Build • Break • Learn"
    RET

SECTION .tech
    DB "C",0,"Lua",0,"Python",0
    DB "JS",0,"TS",0,"HTML",0,"CSS",0,"Tailwind",0
    DB "Vue",0,"React",0,"Node",0,"Django",0,"PHP",0

SECTION .env
    DB "Git",0,"MySQL",0,"npm",0
    DB "Ubuntu",0,"Windows",0

SECTION .interests
    MOV RCX, MATHS
    MOV RDX, PHYSICS

```
