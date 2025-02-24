## online-code-editor

├── backend/                        
│   ├── api-gateway/                # Express, JWT, Authentication
│   ├── services/                   
│   │   ├── user-service/           # User Auth, Profile
│   │   ├── code-execution-service/ # Docker, Sandboxing
│   │   ├── collaboration-service/  # Socket.io, WebRTC
│   │   ├── file-storage-service/   # MongoDB, Redis
│   ├── shared/                     # Logging, DB, Configs
│   ├── Dockerfile                  
│   ├── package.json                
│   ├── tsconfig.json                            
│
├── frontend/                       
│   ├── src/                        
│   │   ├── components/             
│   │   ├── pages/                  # Auth, Dashboard, Editor
│   │   ├── hooks/                  # Custom hooks
│   │   ├── store/                  # Redux 
│   │   ├── utils/                  # Helper functions
│   │   ├── App.tsx                 
│   │   ├── main.tsx                
│   ├── public/                     
│   ├── package.json                              
│   ├── tsconfig.json               
│   ├── Dockerfile                                    
│
├── deployment/                     # DevOps (Kubernetes, CI/CD)
│   ├── k8s/                        
│   ├── docker-compose.yml         
│   ├── nginx/                      
│   ├── github-actions/             
