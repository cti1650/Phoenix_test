FROM elixir:1.15.4-slim

WORKDIR /workspace

RUN apt-get update && apt-get install -y \
    inotify-tools \
    git \
    npm \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

RUN mix local.hex --force && \
	mix archive.install hex phx_new 1.7.7 --force && \
	mix local.rebar --force
