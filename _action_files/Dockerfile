FROM hamelsmu/fastpages-nbdev

WORKDIR /fastpages
COPY . .
RUN chmod u+x action_entrypoint.sh
RUN chmod u+x word2post.sh
RUN dos2unix /fastpages/*.sh

CMD [ "/fastpages/action_entrypoint.sh" ]

ENV GEM_HOME="/usr/local/bundle"
ENV PATH $GEM_HOME/bin:$GEM_HOME/gems/bin:$PATH
