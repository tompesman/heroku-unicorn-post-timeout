# Minimal testcase to trigger the POST timeout at Heroku

ab -n 1 -v 4 -k -T 'application/x-www-form-urlencoded' -H "version: 1.4.9" -H "Accept-Encoding: gzip" -p post.txt http://127.0.0.1:3000/api/v1/games/2248143/move.json