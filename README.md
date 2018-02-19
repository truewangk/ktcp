# ktcp
datagram over tcp
datagram：header +datalen +data
          “ktcp”+len(data)+data
ktcp manager(client) +- tcp sock1 -----------tcp server sock1 -+ ktcp manager(server)
                     +- tcp sock2 -----------tcp server sock2 -+
                     ...
                     +- tcp sockN -----------tcp server sockN -+
