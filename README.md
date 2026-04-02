# AWS Network Architecture (with icons)


```mermaid
flowchart TB

subgraph ACCOUNT[AWS Account]
  subgraph GRP1[" "]
    ELB@{ img: "https://api.iconify.design/logos/aws-elb.svg", label: "ELB", pos: "b", w: 60, h: 60, constraint: "on" }
  end
  subgraph GRP2[" "]
    EC2@{ img: "https://api.iconify.design/logos/aws-ec2.svg", label: "EC2", pos: "b", w: 60, h: 60, constraint: "on" }
  end
  subgraph GRP3[" "]
    RDS@{ img: "https://upload.wikimedia.org/wikipedia/commons/4/4f/SVG_Logo.svg", label: "RDS", pos: "b", w: 60, h: 60, constraint: "on" }
  end
  ELB --- EC2 --- RDS
end

classDef vpc fill:none,color:#0a0,stroke:#0a0
class ACCOUNT vpc

classDef group fill:none,stroke:none
class GRP1,GRP2,GRP3 group
```