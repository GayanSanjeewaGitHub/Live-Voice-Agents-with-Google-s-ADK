# Live-Voice-Agents-with-Google-s-ADK

!adk create --type=code app_01 --model gemini-2.0-flash-live-001 --api_key $GEMINI_API_KEY


cd L1
adk web --host 0.0.0.0 --port 8001


# Kill ADK process
!pkill -f "adk web"



uv venc env --python 3.9.6
pip install -r req.txt
uv pip compile requirements.in -o requirements.txt
