FROM wealdtech/ethdo:1.25.3 as ethdo

FROM attestant/vouch:1.6.2

COPY --from=ethdo /app/ethdo /app/ethdo

RUN apt-get update && apt-get install -y curl jq wget

ENTRYPOINT ["/opt/vouch/run.sh"]