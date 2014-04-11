P6-Digest-HMAC
==============

    use Digest::HMAC;

    # blocksize defaults to 64 (which is correct for sha1 and md5)
    # hash needs to be: sub hash(Buf $in --> Buf)
    my Buf $hmac = hmac($key, $data, &hash, $blocksize);
    my Str $hmac = hmac-hex($key, $data, &hash, $blocksize);
