# agave-sync-demo

This project is inspired by the engineering challenges Agave is working to solve. It’s my attempt to simulate a unified data-sync engine that connects legacy systems, handles multi-tenant workloads fairly, and optimizes caching strategies — all in a practical, hands-on way.

Here’s the high-level feature plan I’m building out:

---

## **1. Webhooks From Scratch**
- API-based “source system” with real webhook subscriptions  
- Legacy DB system with no webhook support → polling + CDC  
- Webhook signing, retry logic, dedupe, event store  
- Unified event schema for all systems  

---

## **2. Fair Background Job System**
- Multi-tenant job queues  
- Token bucket, priority boosting, round-robin scheduling  
- Worker pool simulation  
- Job metrics (latency, fairness, throughput)  

---

## **3. Incremental Cache Optimizer**
- Cache invalidation triggered by webhooks  
- Version-based incremental fetch  
- Diff-based sync  
- Cache metrics + dashboard  

---

I’ll be documenting **every decision I make** — what I researched, why I chose certain approaches, what I learned along the way, and how the design evolved.

My goal is to complete this project in the next **5 weeks**.  
If anyone from the Agave team comes across this, I’d love to connect and chat more about the project!
