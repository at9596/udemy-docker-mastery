FROM jekyll/jekyll:latest
WORKDIR /srv/jekyll

# Copy Gemfile
COPY Gemfile* ./

USER root

# Clean up any existing bundler config and install
RUN bundle config unset frozen && \
    bundle install

RUN chown -R jekyll:jekyll /srv/jekyll

USER jekyll

EXPOSE 4000
CMD ["jekyll", "serve", "--host", "0.0.0.0", "--force_polling"]