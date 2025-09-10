# Space Traffic Management Timeline
```mermaid
%% Swimlane Timeline - Stakeholder + Themes
flowchart TD
    subgraph OPS[Satellite Operators]
        O1[Collect debris data & TLEs -Technical]
        O2[Run propagation to find payloads at risk -Technical]
        O3[Perform/plan maneuvers -Technical/Economic]
    end

    subgraph REG[Regulators / Policy Makers]
        R1[Review technical evidence of risks -Technical/Regulatory]
        R2[Identify gaps in collision prevention -Regulatory]
        R3[Develop coordination frameworks & policies -Regulatory/Social]
    end

    subgraph INS[Insurers / Investors]
        I1[Estimate financial exposure of at-risk payloads -Economic]
        I2[Benchmark historical debris events -Economic]
        I3[Design insurance or mitigation funding mechanisms -Economic/Regulatory]
    end

    subgraph END[End Users / Society]
        S1[Depend on critical services: GPS, telecom, EO -Social]
        S2[Assess disruptions to emergency response, connectivity -Social/Economic]
        S3[Adopt continuity/resilience measures -Social]
    end

    %% Cross-lane dependencies
    O2 --> R1
    O3 --> I1
    I1 --> S2
    R2 --> I3
    R3 --> S3
    S2 --> R3

```


Key Features
Lanes = Stakeholders:
Operators → run data + maneuvers.
Regulators → coordinate rules + policies.
Insurers → model financial risk & create instruments.
End-users → feel the societal/economic impact.
Tagged Themes: Each task explicitly links to Technical / Regulatory / Economic / Social.

Flows:
Operator analysis feeds regulators (for policy) and insurers (for cost).

Insurer risk models inform social impact awareness.

Social disruptions loop back into policy needs.
